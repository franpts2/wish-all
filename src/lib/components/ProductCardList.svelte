<script lang="ts">
	import ProductCard from "./ProductCard.svelte";

	let { products = [] } = $props();
</script>

<div class="overflow-x-auto scrollbar-hide py-4">
	<div class="flex flex-row gap-6">
		{#each products as product}
			<div class="shrink-0">
				<ProductCard
					image={product.image}
					brand={product.brand}
					name={product.name}
				/>
			</div>
		{/each}
	</div>
</div>
