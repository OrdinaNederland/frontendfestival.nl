<script>
	import TagBlock from '$lib/components/TagBlock.svelte';
</script>

<div class="bg-shark text-white py-10 w-full flex-center flex-col" id="schedule">
	<div class="text-4xl px-2">Speaker schedule</div>
	<div class="text-xl px-2">The following schedule is not final and is subject to change.</div>
	<TagBlock class="mt-5" direction="right" extend="true" backgroundColor="fountain">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5 sm:pl-0">16:00</div>
			<div class="text-2xl grow">Welcome</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5">16:30</div>
			<div class="inline-flex flex-col grow">
				<div class="text-2xl">Keynote with Kitze</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5">17:30</div>
			<div class="inline-flex flex-col grow">
				<div class="text-2xl">Firebase</div>
				<div class="text-xl">Frank van Puffelen (Google)</div>
				<div class="text-lg">How you can build better apps faster with Firebase.</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5">17:45</div>
			<div class="inline-flex flex-col grow">
				<div class="text-2xl">AWS & Flutter</div>
				<div class="text-xl">Oscar Hahn (AWS)</div>
				<div class="text-lg">
					Accelerate web and mobile development with AWS Amplify and Flutter.
				</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5">18:00</div>
			<div class="inline-flex flex-col grow">
				<div class="text-2xl">Artistic Bugs</div>
				<div class="text-xl">Jorrik Klijnsma (Ordina)</div>
				<div class="text-lg">When my bug became art; A different perspective.</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="right" extend="true" backgroundColor="fountain">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5 sm:pl-0">18:15</div>
			<div class="text-2xl grow">Drinks & Dinner</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5">19:15</div>
			<div class="inline-flex flex-col grow">
				<div class="text-2xl">Undefined</div>
				<div class="text-lg">Check back later to find out!</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5">19:30</div>
			<div class="inline-flex flex-col grow">
				<div class="text-2xl">Null</div>
				<div class="text-lg">Check back later to find out!</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="right" extend="true" backgroundColor="fountain">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5 sm:pl-0">20:00</div>
			<div class="text-2xl grow">Drinks</div>
		</div>
	</TagBlock>
</div>
