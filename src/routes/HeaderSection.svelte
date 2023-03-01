<script>
	import Poster from '$lib/components/Poster.svelte';
	import TagBlock from '$lib/components/TagBlock.svelte';
</script>

<header class="flex-center w-full h-[85vh] bg-shark relative" id="header">
	<Poster />
	<div class="z-50 flex flex-col justify-center max-h-full text-center">
		<h1 class="block w-screen max-w-3xl p-10">
			<a href="https://frontendfestival.nl">
				<img src="/logo.svg" alt="Frontend Festival Logo" class="" />
			</a>
		</h1>
		<a
			class="inline"
			target="_blank"
			rel="noreferrer"
			href="https://www.eventbrite.com/e/tickets-frontend-festival-522544092447"
		>
			<TagBlock class="text-xl">tickets.getYoursFor<span class="font-bold">Free</span>();</TagBlock>
		</a>
		<a class="inline mt-5" href="#info">
			<TagBlock class="text-xl" backgroundColor="fountain">info.scrollIntoView();</TagBlock>
		</a>
	</div>
</header>
