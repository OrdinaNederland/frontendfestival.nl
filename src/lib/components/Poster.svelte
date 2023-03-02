<script lang="ts">
	import { onMount } from 'svelte';
	import { debounce, random, sample } from 'lodash-es';
	import PosterBall from '$lib/components/PosterBall.svelte';

	const BLUR_RADIUS = 64;
	const BALL_SIZE = [600, 800];
	const SPEED = [50, 70];

	let width;
	let height;
	let balls = [];
	let wrapper: HTMLElement;
	let lastBallId = 0;

	const regenerate = debounce(() => {
		balls = [];
		for (
			let x = Math.floor((-1 * BALL_SIZE[1]) / 400);
			x < Math.ceil((width + BALL_SIZE[1]) / 400);
			x++
		) {
			for (
				let y = Math.floor((-1 * BALL_SIZE[0]) / 400);
				y < Math.ceil((height + BALL_SIZE[0]) / 400);
				y++
			) {
				let xVal = x * 400;
				let yVal = y * 400;
				balls.push(generateBall(random(xVal, xVal + 400), random(yVal, yVal + 400)));
			}
		}
	}, 250);

	function setWidthHeight() {
		width = wrapper.clientWidth;
		height = wrapper.clientHeight;
		regenerate();
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
				'#FF8133'
				// '#FFFFFF'
			]),
			speed: random(SPEED[0], SPEED[1])
		};
	}

	$: console.log(balls.length);

	onMount(() => {
		setWidthHeight();
		window.addEventListener('resize', setWidthHeight);
	});
</script>

<div class="absolute w-full h-full overflow-hidden bg-white z-10 top-0 left-0" bind:this={wrapper}>
	{#each balls as ball, i (ball.id)}
		<PosterBall {...ball} screenWidth={width} on:done={() => (balls[i] = generateBall())} />
	{/each}
</div>
