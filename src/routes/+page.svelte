<script>
	import ProductCard from "$lib/components/ProductCard.svelte";
	import ProductCardList from "$lib/components/ProductCardList.svelte";

	const sampleProducts = [
		{
			image: "/path/to/image.jpg",
			brand: "Brand Name",
			name: "Green wood chair",
		},
		{
			image: "/path/to/image2.jpg",
			brand: "Brand Name",
			name: "Yellow wood chair",
		},
		{
			image: "/path/to/image.jpg",
			brand: "Brand Name",
			name: "Green wood chair",
		},
		{
			image: "/path/to/image2.jpg",
			brand: "Brand Name",
			name: "Yellow wood chair",
		},
		{
			image: "/path/to/image.jpg",
			brand: "Brand Name",
			name: "Green wood chair",
		},
		{
			image: "/path/to/image2.jpg",
			brand: "Brand Name",
			name: "Yellow wood chair",
		},
		{
			image: "/path/to/image.jpg",
			brand: "Brand Name",
			name: "Green wood chair",
		},
		{
			image: "/path/to/image2.jpg",
			brand: "Brand Name",
			name: "Yellow wood chair",
		},
		{
			image: "/path/to/image.jpg",
			brand: "Brand Name",
			name: "Green wood chair",
		},
		{
			image: "/path/to/image2.jpg",
			brand: "Brand Name",
			name: "Yellow wood chair",
		},
	];
</script>

<div>
	<h1 class="text-2xl py-4">Recently Added</h1>
	<ProductCardList products={sampleProducts} />
</div>
