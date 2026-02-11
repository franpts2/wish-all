<script lang="ts">
	const navItems = [
		{ name: "Categories", path: "/categories" },
		{ name: "About", path: "/about" },
	];
</script>

<header class="bg-bg-primary px-8 py-4">
	<div class="flex items-center gap-8">
		<a href="/" class="text-xl font-bold text-text-secondary">Wish All</a>

		<nav class="flex gap-2">
			{#each navItems as item}
				<a
					href={item.path}
					class="px-4 py-2 rounded-lg text-text-primary hover:bg-bg-secondary hover:text-text-primary transition-colors"
				>
					{item.name}
				</a>
			{/each}
		</nav>
	</div>
</header>
