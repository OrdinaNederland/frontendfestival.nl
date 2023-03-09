<script>
	import TagBlock from '$lib/components/TagBlock.svelte';
</script>

<div class="flex-center w-full flex-col bg-western py-10 text-black" id="workshops">
	<div class="px-2 text-4xl">Workshop schedule</div>
	<div class="px-2 text-xl">
		If you want to attend to workshops, you have to register with them as well!
	</div>
	<TagBlock class="mt-5" direction="right" extend="true" backgroundColor="shark">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl sm:pl-0">16:00</div>
			<div class="grow text-2xl">Welcome</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="fountain">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl">16:30</div>
			<div class="inline-flex grow flex-col">
				<div class="text-2xl">Keynote</div>
				<div class="text-xl">Kitze</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="fountain">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl">17:30</div>
			<div class="inline-flex grow flex-col">
				<div class="text-2xl">Start workshops:</div>
				<div class="flex w-full flex-col gap-4">
					<div class="flex grow flex-col">
						<div class="text-xl">- TypeScript</div>
						<div class="text-lg">Davy Engone</div>
						<div>Type Programming with TypeScript.</div>
					</div>
					<div class="flex grow flex-col">
						<div class="text-xl">- Flutter</div>
						<div class="text-lg">Remi Appels (Ordina)</div>
						<div>Creating a review app in 90 minutes using Flutter 3.</div>
					</div>
				</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="right" extend="true" backgroundColor="shark">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl sm:pl-0">18:15</div>
			<div class="grow text-2xl">Drinks & Dinner</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="fountain">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl">19:15</div>
			<div class="inline-flex grow flex-col">
				<div class="text-2xl">Continuation workshops</div>
				<div>You're going back to the same workshop from before the break.</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="right" extend="true" backgroundColor="shark">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl sm:pl-0">20:15</div>
			<div class="grow text-2xl">Drinks</div>
		</div>
	</TagBlock>
</div>
