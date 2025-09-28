<script lang="ts">
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";

	let {
		title,
		subtitle,
		imageSrc = "https://www.unc.mn/image-placeholder.svg",
		...rest
	}: {
		title: string;
		subtitle: string;
		imageSrc: string;
		[key: string]: any;
	} = $props();
</script>

<header class={[
	"relative overflow-hidden border-b border-gray-100 dark:border-gray-900",
	"bg-gradient-to-br from-primary-600 via-primary-500 to-secondary-500"
]} {...rest}>
	<div class="text-title3 section-px section-py container mx-auto grid gap-16 gap-y-0 relative z-10">
		<div class="text-center text-white">
			<h1 class="text-display font-medium mb-6 leading-tight">{title}</h1>
			<p class="text-title2 opacity-90 leading-relaxed">{subtitle}</p>
		</div>
		<div class="aspect-video overflow-clip rounded-xl bg-white/10 backdrop-blur-sm border border-white/20">
			<img
				class="h-full w-full object-cover rounded-xl"
				src={imageSrc}
				alt="Professional team analyzing market data"
			/>
		</div>
	</div>
	<!-- Subtle gradient overlay for depth -->
	<div class="absolute inset-0 bg-gradient-to-t from-black/5 via-transparent to-white/5 pointer-events-none"></div>
</header>
