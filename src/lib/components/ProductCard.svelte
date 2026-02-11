<script lang="ts">
    let {
        image = "",
        brand = "",
        name = "",
        rating = 0,
        reviewCount = 0,
        price = 0,
    } = $props();
</script>

<div class="w-xs overflow-hidden rounded-lg hover:shadow-lg transition-shadow">
    <!-- Product Image -->
    <div class="aspect-square rounded-lg bg-bg-tertiary overflow-hidden">
        <img src={image} alt={name} class="w-full h-full object-cover" />
    </div>

    <!-- Product Info -->
    <div class="p-4 space-y-1">
        <!-- Brand -->
        <p class="text-sm text-text-secondary">{brand}</p>

        <!-- Product Name -->
        <h3 class="font-medium text-text-primary">{name}</h3>

        <!-- Rating -->
        <div class="flex items-center gap-2">
            <div class="flex items-center">
                <span class="text-sm">⭐</span>
                <span class="text-sm font-medium text-text-primary ml-1">{rating}</span>
            </div>
            <span class="text-sm text-text-secondary">({reviewCount})</span>
        </div>

        <!-- Price -->
        <p class="text-lg font-bold text-text-primary">${price}</p>
    </div>
</div>
