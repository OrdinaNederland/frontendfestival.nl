<script>
	import TagBlock from '$lib/components/TagBlock.svelte';
</script>

<div class="bg-shark text-white py-10 w-full flex-center flex-col" id="practical-information">
	<div class="text-4xl">Practical information</div>

	<TagBlock class="mt-5" direction="right" extend="true" backgroundColor="ordina">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5 sm:pl-0">When:</div>
			<div class="text-2xl grow">April 13th 2023, 16:00 - 22:00</div>
		</div>
	</TagBlock>

	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="fountain">
		<div class="flex gap-5 w-screen max-w-xl items-center">
			<div class="text-2xl pl-5" />
			<div class="flex flex-col md:flex-row gap-2 items-center">
				<a target="_blank" rel="noreferrer" href="https://goo.gl/maps/xumZR7ZQR53VJTQk7"
					><img
						class="w-48 h-48 p-1 rounded-full ring-2 ring-fountain-300"
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

	<div class="text-xl mt-10">Limited places available, so hurry up!</div>

	<a
		class="inline mt-5"
		target="_blank"
		rel="noreferrer"
		href="https://www.eventbrite.com/e/tickets-frontend-festival-522544092447"
	>
		<TagBlock class="text-xl">tickets.getYoursFor<span class="font-bold">Free</span>();</TagBlock>
	</a>
</div>
