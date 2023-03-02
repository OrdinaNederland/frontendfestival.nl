<script lang="ts">
	import { createEventDispatcher, onMount } from 'svelte';
	import { random } from 'lodash-es';

	const dispatch = createEventDispatcher();

	const BLUR_RADIUS = 64;

	export let animated: boolean = false;
	export let backgroundColor;
	export let size;
	export let zIndex;
	export let top;
	export let left;
	export let screenWidth;
	export let speed;

	let endTop = 0;
	let endLeft = 0;
	let transitionTime = 0;
	let started = false;

	onMount(() => {
		endTop = top + random(-500, 500);
		endLeft = screenWidth + BLUR_RADIUS + size;
		transitionTime = Math.round(((endLeft - left) / speed) * 1000);

		let timeout;
		if (screenWidth > 768 || !animated) {
			timeout = setTimeout(() => {
				started = true;
				timeout = setTimeout(() => {
					dispatch('done');
				}, transitionTime);
			}, 5);
		}

		return () => {
			clearTimeout(timeout);
		};
	});
</script>

<div
	class="ball"
	class:started={started && screenWidth > 768 && animated}
	style="
	  --blurRadius: {BLUR_RADIUS};
    --backgroundColor: {backgroundColor};
    --size: {size}px;
    --zIndex: {zIndex};
    --startTop: {top}px;
    --startLeft: {left}px;
    --endTop: {endTop}px;
    --endLeft: {endLeft}px;
    --transitionTime: {transitionTime}ms;
  "
/>

<style lang="postcss">
	.ball {
		@apply absolute pointer-events-none blur-3xl rounded-full;
		background-color: var(--backgroundColor);
		width: var(--size);
		height: var(--size);
		top: var(--startTop);
		left: var(--startLeft);
		z-index: var(--zIndex);
		transition-property: top, left;

		&.started {
			transition-duration: var(--transitionTime);
			transition-timing-function: linear;
			top: var(--endTop);
			left: var(--endLeft);
		}
	}
</style>
