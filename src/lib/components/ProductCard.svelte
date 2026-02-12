<script lang="ts">
	let {
		image = "",
		brand = "",
		name = "",
	} = $props();
</script>

<div
	class="w-60 overflow-hidden rounded-lg cursor-pointer hover:shadow-lg transition-all duration-300 hover:-translate-y-2 hover:scale-[1.02]"
>
	<!-- Product Image -->
	<div
		class="aspect-square rounded-lg bg-bg-tertiary overflow-hidden relative group"
	>
		<img src={image} alt={name} class="w-full h-full object-cover" />
	</div>

	<!-- Product Info -->
	<div class="p-4 space-y-1">
		<!-- Brand -->
		<p class="text-sm text-text-secondary">{brand}</p>

		<!-- Product Name -->
		<h3 class="font-medium text-text-primary">{name}</h3>
	</div>
</div>
