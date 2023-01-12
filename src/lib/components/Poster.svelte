<script lang="ts">
	import { onMount } from 'svelte';
	import { random, sample } from 'lodash-es';

	const BLUR_RADIUS = 64;
	const BALL_SIZE = [400, 600];

	let width;
	let height;
	let balls = [];
	let wrapper: HTMLElement;
	let lastBallId = 0;
	let animationFrame: number;

	function move() {
		// Moving them all at once, for performance.
		// In-place mutation of the balls array makes Svelte draw them one-by-one.
		let newBalls = [...balls];
		newBalls.forEach((ball, ballIndex) => {
			if (
				ball.left < width + ball.size + BLUR_RADIUS &&
				ball.top < height + ball.size + BLUR_RADIUS
			) {
				ball.left += ball.speed / 10;
				ball.top += ball.yMove * (1 / ball.speed);
			} else {
				newBalls[ballIndex] = generateBall();
			}
		});
		balls = newBalls;

		animationFrame = requestAnimationFrame(move);
	}

	function setWidthHeight() {
		width = wrapper.clientWidth;
		height = wrapper.clientHeight;
	}

	function generateBall(left?: number, top?: number) {
		let size = random(BALL_SIZE[0], BALL_SIZE[1]);
		return {
			id: lastBallId++,
			top: top ?? random(0, height),
			left: left ?? -1 * BLUR_RADIUS - size,
			size: size,
			zIndex: random(0, 100),
			backgroundColor: sample([
				'#1A1D1F',
				'#61BFC3',
				'#61BFC3',
				'#E6E2DB',
				'#FF8133',
				'#FF8133',
				'#FFFFFF'
			]),
			speed: random(5, 15),
			yMove: random(-1, 1, true)
		};
	}

	onMount(() => {
		setWidthHeight();
		window.addEventListener('resize', setWidthHeight);

		for (
			let x = Math.floor((-1 * BALL_SIZE[1]) / 200);
			x < Math.ceil((width + BALL_SIZE[1]) / 200);
			x++
		) {
			for (
				let y = Math.floor((-1 * BALL_SIZE[0]) / 200);
				y < Math.ceil((height + BALL_SIZE[0]) / 200);
				y++
			) {
				let xVal = x * 200;
				let yVal = y * 200;
				balls.push(generateBall(random(xVal, xVal + 200), random(yVal, yVal + 200)));
			}
		}

		animationFrame = requestAnimationFrame(move);
		return () => cancelAnimationFrame(animationFrame);
	});
</script>

<div class="absolute w-full h-full overflow-hidden bg-white z-10 top-0 left-0" bind:this={wrapper}>
	{#each balls as ball, i (ball.id)}
		<div
			class="absolute pointer-events-none blur-3xl rounded-full"
			style="background-color: {ball.backgroundColor}; width: {ball.size}px; height: {ball.size}px; z-index: {ball.zIndex}; top: {ball.top}px; left: {ball.left}px;"
		/>
	{/each}
</div>
