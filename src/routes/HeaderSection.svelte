<script>
	import Poster from '$lib/components/Poster.svelte';
	import TagBlock from '$lib/components/TagBlock.svelte';
	import { Icon } from 'svelte-awesome';
	import { chevronDown } from 'svelte-awesome/icons';
</script>

<header class="flex-center relative h-[85vh] w-full bg-shark" id="header">
	<Poster animated />
	<div class="z-50 flex max-h-full flex-col justify-center text-center">
		<h1 class="block w-screen max-w-4xl px-5 py-20">
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
			<TagBlock class="text-lg" backgroundColor="fountain">
				tickets.getYoursFor<span class="font-bold">Free</span>();
			</TagBlock>
		</a>
		<div class="flex-center absolute bottom-0 left-0 w-full">
			<a class="mb-10 inline" href="#info">
				<Icon class="text-white opacity-75" data={chevronDown} scale="3" />
			</a>
		</div>
	</div>
</header>
