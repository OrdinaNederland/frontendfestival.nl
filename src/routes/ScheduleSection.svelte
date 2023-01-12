<script>
	import TagBlock from '$lib/components/TagBlock.svelte';
</script>

<div class="bg-shark text-white py-10 w-full flex-center flex-col" id="schedule">
	<div class="text-4xl">Schema</div>
	<TagBlock class="mt-5" direction="right" extend="true" backgroundColor="fountain">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl">16:00</div>
			<div class="text-2xl grow">Ontvangst</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5">16:30</div>
			<div class="inline-flex flex-col grow">
				<div class="text-xl">Keynote</div>
				<div class="col-start-2">Some information about the keynote</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5">17:30</div>
			<div class="inline-flex flex-col grow">
				<div class="text-2xl">Parallel sessie 1</div>
				<div class="flex flex-col lg:flex-row w-full gap-2">
					<div class="grow flex flex-col">
						<div class="text-xl">Sessie A</div>
						<div>Info over Sessie A</div>
					</div>
					<div class="grow flex flex-col">
						<div class="text-xl">Sessie B</div>
						<div>Info over Sessie B</div>
					</div>
				</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="right" extend="true" backgroundColor="fountain">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl">18:15</div>
			<div class="text-2xl grow">Drinks & Dinner</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5">19:15</div>
			<div class="inline-flex flex-col grow">
				<div class="text-2xl">Parallel sessie 2</div>
				<div class="flex flex-col lg:flex-row w-full gap-2">
					<div class="grow flex flex-col">
						<div class="text-xl">Sessie A</div>
						<div>Info over Sessie A</div>
					</div>
					<div class="grow flex flex-col">
						<div class="text-xl">Sessie B</div>
						<div>Info over Sessie B</div>
					</div>
				</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="right" extend="true" backgroundColor="fountain">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl">20:00</div>
			<div class="text-2xl grow">Drinks</div>
		</div>
	</TagBlock>
</div>
