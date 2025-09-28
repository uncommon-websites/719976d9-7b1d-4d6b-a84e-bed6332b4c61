<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Real-time insights",
			description: "We believe data should flow at the speed of business. While traditional research takes weeks, we deliver instant validation by analyzing billions of consumer signals in real-time."
		},
		{
			title: "Behavioral truth",
			description: "What people do matters more than what they say. We capture actual consumer behavior across platforms and channels, not hypothetical survey responses."
		},
		{
			title: "Democratized intelligence",
			description: "Market research shouldn't be exclusive to enterprise budgets. We're making sophisticated consumer insights accessible to fast-growing brands at every stage."
		}
	];
</script>

<SecondaryHero
	title="Decisions backed by reality"
	subtitle="Built for fast-moving consumer brands"
	imageSrc="/generated/image-a-professional-team-of-diverse-adults-ga.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Product managers at fast-growing consumer brands face an impossible choice: wait weeks for traditional market research that costs thousands, or make critical product decisions based on gut feeling while competitors surge ahead. We witnessed brilliant teams with game-changing ideas held back by outdated research methods that couldn't keep pace with modern product development cycles.",
		"That's why we built &facts to analyze billions of real-world consumer behavior signals and deliver instant market validation in minutes, not months. Instead of relying on what people say they'll do in surveys, we capture what they're actually doing across social platforms, search engines, and shopping behaviors to give product teams the reliable data they need to move fast with confidence.",
		"Today, &facts is transforming how consumer brands validate new concepts, helping teams run 10,000+ validation reports monthly and make data-backed decisions at the speed of business. We're not just changing market research—we're enabling a new era where the best ideas win because teams can test, learn, and iterate faster than ever before."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Meet the founder."
	subtitle="Building the future of market research."
	stakeholders={[
		{
			name: "Sohaib Ahmed",
			position: "Founder & CEO",
			bio: "Built &facts to give product teams the speed and certainty they need to win in competitive markets.",
			image: "/generated/image-a-professional-headshot-of-a-business-ex.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Stop waiting weeks for answers"
	subtitle="Get instant market validation"
	description="Join product managers at fast-growing consumer brands who trust &facts to validate concepts with real consumer behavior data. Transform your decision-making from weeks to minutes."
	imageSrc="/generated/image-a-professional-product-manager-sits-at-a.webp"
/>
