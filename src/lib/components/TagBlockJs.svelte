<script lang="ts">
	import { onMount } from 'svelte';

	export let backgroundColor: 'shark' | 'fountain' | 'ordina' = 'ordina';
	export let direction: 'left' | 'right' | 'both' = 'both';

	let leftArrowElement: HTMLElement | null;
	let rightArrowElement: HTMLElement | null;
	let contentElement: HTMLElement;

	function setArrowSize() {
		if (leftArrowElement) {
			leftArrowElement.style.height = '0';
		}
		if (rightArrowElement) {
			rightArrowElement.style.height = '0';
		}

		let height = contentElement.clientHeight;

		if (leftArrowElement) {
			leftArrowElement.style.height = `${height}px`;
		}
		if (rightArrowElement) {
			rightArrowElement.style.height = `${height}px`;
		}
	}

	onMount(() => {
		setArrowSize();
		window.addEventListener('resize', setArrowSize);
	});
</script>

<div class="text-white flex relative">
	{#if ['left', 'both'].indexOf(direction) > -1}
		<svg
			bind:this={leftArrowElement}
			viewBox="0 0 71 100"
			xml:space="preserve"
			xmlns="http://www.w3.org/2000/svg"
		>
			<g transform="matrix(3.7761 0 0 3.7761 -8.9107 .10595)">
				<path
					d="m21.162 26.454c-0.52053-0.0026-0.95771-0.03192-1.278-0.08895v1e-6c-1.1306-0.2013-2.0481-0.56897-2.9909-1.1985-0.24707-0.16498-1.8467-1.4021-3.5548-2.7492s-3.4603-2.7247-3.8939-3.0613c-1.2783-0.9926-6.6053-5.2037-6.753-5.3385-0.4013-0.36609-0.44538-1.0491-0.094261-1.4605 0.047677-0.05586 1.9142-1.5427 4.1478-3.304s5.3979-4.26 7.0318-5.5526c3.1588-2.499 3.5686-2.7866 4.5013-3.1586 1.0008-0.39926 1.7501-0.5685 2.8839-0.56991"
					fill="#ff8133"
				/>
			</g>
		</svg>
	{/if}
	<div
		bind:this={contentElement}
		class="py-4 inline"
		class:bg-ordina={backgroundColor === 'ordina'}
		class:pl-4={direction === 'right'}
		class:pr-4={direction === 'left'}
	>
		<slot />
	</div>
	{#if ['right', 'both'].indexOf(direction) > -1}
		<svg
			bind:this={rightArrowElement}
			viewBox="0 0 71 100"
			xml:space="preserve"
			xmlns="http://www.w3.org/2000/svg"
		>
			<g transform="matrix(-3.7761 0 0 3.7761 79.911 .10595)">
				<path
					d="m21.162 26.454c-0.52053-0.0026-0.95771-0.03192-1.278-0.08895v1e-6c-1.1306-0.2013-2.0481-0.56897-2.9909-1.1985-0.24707-0.16498-1.8467-1.4021-3.5548-2.7492s-3.4603-2.7247-3.8939-3.0613c-1.2783-0.9926-6.6053-5.2037-6.753-5.3385-0.4013-0.36609-0.44538-1.0491-0.094261-1.4605 0.047677-0.05586 1.9142-1.5427 4.1478-3.304s5.3979-4.26 7.0318-5.5526c3.1588-2.499 3.5686-2.7866 4.5013-3.1586 1.0008-0.39926 1.7501-0.5685 2.8839-0.56991"
					fill="#ff8133"
					stroke-width=".047639"
				/>
			</g>
		</svg>
	{/if}
</div>
