<script>
	import TagBlock from '$lib/components/TagBlock.svelte';
</script>

<div class="w-full py-10 bg-fountain text-black" id="speakers">
	<div class="text-4xl w-full text-center mb-5">Speakers</div>
	<div class="w-full max-w-6xl m-auto">
		<TagBlock class="max-w-lg float-right" direction="left" extend="true">
			<div class="flex flex-col w-full">
				<div class="flex grow items-center gap-2">
					<div
						class="relative inline-flex items-center justify-center w-14 h-14 overflow-hidden rounded-full bg-fountain"
					>
						<span class="font-medium text-fountain-800 text-2xl">KI</span>
					</div>
					<div class="flex flex-col grow">
						<div class="text-2xl">Kitze</div>
						<div class="text-xl">Undefined @ Null</div>
					</div>
				</div>
				<div>
					Uncaught TypeError: Cannot read properties of undefined (reading 'bioKitze') - Coming
					soon!
				</div>
			</div>
		</TagBlock>

		<TagBlock
			class="max-w-lg float-left mt-5 lg:mt-24"
			direction="right"
			backgroundColor="shark"
			extend="true"
		>
			<div class="flex flex-col w-full">
				<div class="flex grow items-center gap-2">
					<img
						class="h-14 w-14 aspect-square rounded-full"
						src="/speakers/fvp.png"
						alt="Frank van Puffelen"
					/>
					<div class="flex flex-col grow">
						<div class="text-2xl">Frank van Puffelen / puf</div>
						<div class="text-xl">Firebase engineer @ Google</div>
					</div>
				</div>
				<div>
					Frank van Puffelen (puf) is a Firebase engineer at Google in San Francisco, where he helps
					developers build better apps using Firebase and other Google technologies. He's the host
					of the Firebase Release Notes video series, one of the top contributors on Stack Overflow,
					and multi-time speaker at Google I/O.
				</div>
			</div>
		</TagBlock>

		<TagBlock class="max-w-lg float-right mt-5 lg:mt-36" direction="left" extend="true">
			<div class="flex flex-col w-full">
				<div class="flex grow items-center gap-2">
					<div
						class="relative inline-flex items-center justify-center w-14 h-14 overflow-hidden rounded-full bg-fountain"
					>
						<span class="font-medium text-fountain-800 text-2xl">DE</span>
					</div>
					<div class="flex flex-col grow">
						<div class="text-2xl">Davy Engone</div>
						<div class="text-xl">Undefined @ Null</div>
					</div>
				</div>
				<div>
					Uncaught TypeError: Cannot read properties of undefined (reading 'bioDavyEngone') - Coming
					soon!
				</div>
			</div>
		</TagBlock>

		<TagBlock
			class="max-w-lg float-left mt-5 lg:mt-10"
			direction="right"
			backgroundColor="shark"
			extend="true"
		>
			<div class="flex flex-col w-full">
				<div class="flex grow items-center gap-2">
					<img
						class="h-14 w-14 aspect-square rounded-full"
						src="/speakers/oh.png"
						alt="Oscar Hahn"
					/>
					<div class="flex flex-col grow">
						<div class="text-2xl">Oscar Hahn</div>
						<div class="text-xl">Solutions Architect @ AWS</div>
					</div>
				</div>
				<div>
					Oscar is a cloud computing expert with experience in building serverless (web)
					applications using CI/CD principles. In his current Solutions Architect role at AWS he is
					advising and guiding customers in designing and implementing cloud based solutions to
					optimise their business operations.
				</div>
			</div>
		</TagBlock>

		<TagBlock class="max-w-lg float-right mt-5 lg:mt-32" direction="left" extend="true">
			<div class="flex flex-col w-full">
				<div class="flex grow items-center gap-2">
					<img
						class="h-14 w-14 aspect-square rounded-full"
						src="/speakers/rs.png"
						alt="Robbin Schepers"
					/>
					<div class="flex flex-col grow">
						<div class="text-2xl">Robbin Schepers / Roboroads</div>
						<div class="text-xl">Senior Software Engineer @ Ordina</div>
					</div>
				</div>
				<div>
					Robbin Schepers is a Professional Computer Nerd and has a deep love for everythiong
					computer and tech related. He is a Senior Software Engineer at Ordina since 2021,
					freelancer since 2013 and even public speaker since 2022. He loves representing tech
					stacks that use the least amount of code whilst still being fully functional like Flutter
					and Svelte. He also created this website in SvelteKit!
				</div>
			</div>
		</TagBlock>

		<TagBlock
			class="max-w-lg float-left mt-5 lg:mt-48"
			direction="right"
			backgroundColor="shark"
			extend="true"
		>
			<div class="flex flex-col w-full">
				<div class="flex grow items-center gap-2">
					<img
						class="h-14 w-14 aspect-square rounded-full"
						src="/speakers/jk.png"
						alt="Oscar Hahn"
					/>
					<div class="flex flex-col grow">
						<div class="text-2xl">Jorrik Kleinsma</div>
						<div class="text-xl">Software Engineer @ Ordina</div>
					</div>
				</div>
				<div>
					Jorrik’s first lines of code were in the days jQuery ruled. That didn’t scare him. Now he
					has 6+ years of frontend experience using React and Vue during his day job. In the evening
					and night hours, a lot of fun projects and other libraries passed his ‘git clone’. When
					not coding he gets his fair share of laughs going to comedy shows.
				</div>
			</div>
		</TagBlock>
	</div>
	<div class="clear-both" />
</div>
