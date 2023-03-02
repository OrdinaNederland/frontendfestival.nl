<script lang="ts">
	import '../reset.pcss';
	import '../tailwind.pcss';
</script>

<div class="flex h-screen w-screen flex-col overflow-x-hidden">
	<div class="min-h-screen overflow-x-hidden scroll-smooth">
		<slot />
	</div>
</div>
