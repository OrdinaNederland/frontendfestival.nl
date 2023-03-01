<script>
	import TagBlock from '$lib/components/TagBlock.svelte';
</script>

<div class="bg-western text-black py-10 w-full flex-center flex-col" id="workshops">
	<div class="text-4xl px-2">Workshop schedule</div>
	<div class="text-xl px-2">
		If you want to attend to workshops, you have to register with them as well!
	</div>
	<TagBlock class="mt-5" direction="right" extend="true" backgroundColor="shark">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5 sm:pl-0">16:00</div>
			<div class="text-2xl grow">Welcome</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="fountain">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5">16:30</div>
			<div class="inline-flex flex-col grow">
				<div class="text-2xl">Keynote</div>
				<div class="text-xl">Kitze</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="fountain">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5">17:30</div>
			<div class="inline-flex flex-col grow">
				<div class="text-2xl">Start workshops:</div>
				<div class="flex flex-col w-full gap-4">
					<div class="grow flex flex-col">
						<div class="text-xl">- TypeScript</div>
						<div class="text-lg">Davy Engone</div>
						<div>Type Programming with TypeScript.</div>
					</div>
					<div class="grow flex flex-col">
						<div class="text-xl">- Flutter</div>
						<div class="text-lg">Robbin Schepers (Ordina)</div>
						<div>Creating a review app in 90 minutes using Flutter 3.</div>
					</div>
				</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="right" extend="true" backgroundColor="shark">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5 sm:pl-0">18:15</div>
			<div class="text-2xl grow">Drinks & Dinner</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="fountain">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5">19:15</div>
			<div class="inline-flex flex-col grow">
				<div class="text-2xl">Continuation workshops</div>
				<div>You're going back to the same workshop from before the break.</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="right" extend="true" backgroundColor="shark">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5 sm:pl-0">20:00</div>
			<div class="text-2xl grow">Drinks</div>
		</div>
	</TagBlock>
</div>
