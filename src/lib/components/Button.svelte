<script lang="ts">
	export let variant: "primary" | "secondary" = "primary";
	export let iconPosition: "left" | "right" | "none" = "none";
	export let icon: string = "";
	export let type: "button" | "submit" | "reset" = "button";
	export let disabled: boolean = false;

	const baseClasses =
		"z-100 inline-flex items-center justify-center gap-2.5 px-4 py-2 rounded-2xl text-lg font-medium cursor-pointer transition-all duration-200 border-none whitespace-nowrap disabled:opacity-50 disabled:cursor-not-allowed";

	const variantClasses = {
		secondary:
			"bg-bg-primary text-text-primary border-2 border-brand-greige shadow-sm hover:bg-bg-secondary hover:border-brand-stone hover:shadow-md active:bg-brand-greige active:translate-y-px",
		primary:
			"bg-gradient-to-br from-accent-gold to-accent-primary text-text-inverse shadow-lg shadow-accent-primary/30 hover:from-accent-gold/90 hover:to-accent-primary/90 hover:shadow-xl hover:shadow-accent-primary/40 hover:-translate-y-px active:from-accent-primary active:to-accent-secondary active:translate-y-0",
	};
</script>

<button
	class="{baseClasses} {variantClasses[variant]}"
	{type}
	{disabled}
	on:click
>
	{#if iconPosition === "left" && icon}
		<span class="inline-flex items-center justify-center text-xl"
			>{@html icon}</span
		>
	{/if}
	<span class="inline-flex items-center">
		<slot />
	</span>
	{#if iconPosition === "right" && icon}
		<span class="inline-flex items-center justify-center text-xl"
			>{@html icon}</span
		>
	{/if}
</button>
