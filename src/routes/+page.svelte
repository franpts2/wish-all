<script>
	import Button from "$lib/components/Button.svelte";
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

	const addIcon =
		'<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6"><path stroke-linecap="round" stroke-linejoin="round" d="M12 4.5v15m7.5-7.5h-15" /></svg>';
</script>

<div>
	<div class="flex flex-row items-center justify-between">
		<h1 class="text-2xl py-4">Recently Added</h1>
		<Button iconPosition="left" icon={addIcon}>Add More</Button>
	</div>
	<ProductCardList products={sampleProducts} />
</div>
