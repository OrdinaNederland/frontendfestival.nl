<script lang="ts">
	import '../reset.pcss';
	import '../tailwind.pcss';
</script>

<div class="flex flex-col overflow-x-hidden w-screen h-screen">
	<div class="min-h-screen overflow-x-hidden">
		<slot />
	</div>
</div>
