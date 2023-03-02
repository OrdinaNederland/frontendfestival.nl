<script>
	import TagBlock from '$lib/components/TagBlock.svelte';
</script>

<div class="flex-center w-full flex-col bg-shark py-10 text-white" id="schedule">
	<div class="px-2 text-4xl">Speaker schedule</div>
	<div class="px-2 text-xl">The following schedule is not final and is subject to change.</div>
	<TagBlock class="mt-5" direction="right" extend="true" backgroundColor="fountain">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl sm:pl-0">16:00</div>
			<div class="grow text-2xl">Welcome</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl">16:30</div>
			<div class="inline-flex grow flex-col">
				<div class="text-2xl">Keynote with Kitze</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl">17:30</div>
			<div class="inline-flex grow flex-col">
				<div class="text-2xl">Firebase</div>
				<div class="text-xl">Frank van Puffelen (Google)</div>
				<div class="text-lg">How you can build better apps faster with Firebase.</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl">17:45</div>
			<div class="inline-flex grow flex-col">
				<div class="text-2xl">AWS & Flutter</div>
				<div class="text-xl">Oscar Hahn (AWS)</div>
				<div class="text-lg">
					Accelerate web and mobile development with AWS Amplify and Flutter.
				</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl">18:00</div>
			<div class="inline-flex grow flex-col">
				<div class="text-2xl">Artistic Bugs</div>
				<div class="text-xl">Jorrik Klijnsma (Ordina)</div>
				<div class="text-lg">When my bug became art; A different perspective.</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="right" extend="true" backgroundColor="fountain">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl sm:pl-0">18:15</div>
			<div class="grow text-2xl">Drinks & Dinner</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl">19:15</div>
			<div class="inline-flex grow flex-col">
				<div class="text-2xl">Undefined</div>
				<div class="text-lg">Check back later to find out!</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl">19:30</div>
			<div class="inline-flex grow flex-col">
				<div class="text-2xl">Null</div>
				<div class="text-lg">Check back later to find out!</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="right" extend="true" backgroundColor="fountain">
		<div class="flex w-screen max-w-xl gap-5">
			<div class="pl-5 text-2xl sm:pl-0">20:00</div>
			<div class="grow text-2xl">Drinks</div>
		</div>
	</TagBlock>
</div>
