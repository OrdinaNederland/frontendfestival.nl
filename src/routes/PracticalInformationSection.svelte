<script>
	import TagBlock from '$lib/components/TagBlock.svelte';
</script>

<div
	class="flex-center relative w-full flex-col bg-shark py-10 text-white"
	id="practical-information"
>
	<div class="text-4xl">Practical information</div>

	<TagBlock class="mt-5" direction="right" extend="true" backgroundColor="ordina">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl sm:pl-0">When:</div>
			<div class="grow text-2xl">April 13th 2023, 16:00 - 22:00</div>
		</div>
	</TagBlock>

	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="fountain">
		<div class="flex w-screen max-w-xl items-center gap-5">
			<div class="pl-5 text-2xl" />
			<div class="flex flex-col items-center gap-2 md:flex-row">
				<a target="_blank" rel="noreferrer" href="https://goo.gl/maps/xumZR7ZQR53VJTQk7"
					><img
						class="h-48 w-48 rounded-full p-1 ring-2 ring-fountain-300"
						src="/map.png"
						alt="A map showing where Ordina is located, on the line between Nieuwegein and Utrecht"
					/></a
				>
				<div class="flex flex-col">
					<div class="text-2xl">Where: Ordina HQ</div>
					<div class="text-xl">Ringwade 1</div>
					<div class="text-xl">3439 LM Nieuwegein</div>
					<div class="text-xl">The Netherlands</div>
				</div>
			</div>
		</div>
	</TagBlock>

	<div class="mt-10 text-xl">Limited places available, so hurry up!</div>

	<a
		class="mt-5 inline"
		target="_blank"
		rel="noreferrer"
		href="https://www.eventbrite.com/e/tickets-frontend-festival-522544092447"
	>
		<TagBlock class="text-xl">tickets.getYoursFor<span class="font-bold">Free</span>();</TagBlock>
	</a>

	<a
		class="mt-10 inline"
		target="_blank"
		rel="noreferrer"
		href="https://github.com/OrdinaNederland/frontendfestival.nl"
	>
		<TagBlock backgroundColor="fountain" small>Source on GitHub</TagBlock>
	</a>
</div>
