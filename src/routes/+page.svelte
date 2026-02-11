<script>
	import ProductCard from "$lib/components/ProductCard.svelte";
</script>

<div>
	<h1 class="text-accent-primary">Home page</h1>

	<ProductCard
		image="https://example.com/hoodie.jpg"
		brand="Brand Name"
		name="Product Name"
		rating={4.2}
		reviewCount={12}
		price={50}
	/>
</div>
