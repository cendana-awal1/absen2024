<script>
	import KelasA from '../lib/KelasA.svelte';
	import data from '../lib/data.json';
</script>

<!-- container tilwindcss -->
<div class="justify-between grid grid-cols-1 gap-8 md:grid-cols-2 lg:grid-cols-3 xl:gap-12 max-w-6xl mx-auto px-4 py-12">
	<div class="grid grid-cols-4 gap-2 mb-3">
		{#each data as item}
			<KelasA {item} />
		{/each}
	</div>
</div>
