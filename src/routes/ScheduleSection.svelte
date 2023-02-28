<script>
	import TagBlock from '$lib/components/TagBlock.svelte';
</script>

<div class="bg-shark text-white py-10 w-full flex-center flex-col" id="schedule">
	<div class="text-4xl">Speaker schedule</div>
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
				<div class="text-xl">Keynote with Kitze</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5">17:30</div>
			<div class="inline-flex flex-col grow">
				<div class="text-2xl">First parallel sessions</div>
				<div class="flex flex-col lg:flex-row w-full gap-4">
					<div class="grow flex flex-col">
						<div class="text-xl">1. Frank van Puffelen (Google)</div>
						<div>How you can build better apps faster with Firebase.</div>
					</div>
					<div class="grow flex flex-col">
						<div class="text-xl">2. Oscar Hahn (AWS)</div>
						<div>Accelerate web and mobile development with AWS Amplify and Flutter.</div>
					</div>
					<div class="grow flex flex-col">
						<div class="text-xl">3. Jorrik Kleinsma (Ordina)</div>
						<div>When my bug became art; A different perspective.</div>
					</div>
				</div>
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
			<div class="text-2xl pl-5 sm:pl-0">20:00</div>
			<div class="text-2xl grow">Drinks</div>
		</div>
	</TagBlock>
</div>

<div class="bg-fountain text-white py-10 w-full flex-center flex-col" id="workshops">
	<div class="text-4xl">Workshop schedule</div>
	<div class="text-xl">
		If you want to attend to workshops, you have to register with them as well!
	</div>
	<TagBlock class="mt-5" direction="right" extend="true" backgroundColor="shark">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5 sm:pl-0">16:00</div>
			<div class="text-2xl grow">Welcome</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5">16:30</div>
			<div class="inline-flex flex-col grow">
				<div class="text-xl">Keynote with Kitze</div>
			</div>
		</div>
	</TagBlock>
	<TagBlock class="mt-2" direction="left" extend="true" backgroundColor="ordina">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5">17:30</div>
			<div class="inline-flex flex-col grow">
				<div class="text-2xl">Workshops - first half</div>
				<div class="flex flex-col lg:flex-row w-full gap-4">
					<div class="grow flex flex-col">
						<div class="text-xl">1. Robbin Schepers</div>
						<div>Creating an app in 60 minutes with Flutter 3.</div>
					</div>
					<div class="grow flex flex-col">
						<div class="text-xl">2. Davy Engone</div>
						<div>Type Programming with TypeScript.</div>
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
	<TagBlock class="mt-2" direction="right" extend="true" backgroundColor="shark">
		<div class="flex gap-5 w-screen max-w-xl">
			<div class="text-2xl pl-5 sm:pl-0">20:00</div>
			<div class="text-2xl grow">Drinks</div>
		</div>
	</TagBlock>
</div>
