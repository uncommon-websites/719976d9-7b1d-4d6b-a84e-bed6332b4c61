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
			title: "Speed",
			description: "Delivering market insights in minutes, not weeks, because fast decisions win."
		},
		{
			title: "Accuracy",
			description: "Analyzing real consumer behavior, not survey responses, for reliable validation."
		},
		{
			title: "Impact",
			description: "Empowering product teams to make confident decisions that drive business growth."
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
	title="Our team."
	subtitle="Your partners in market intelligence."
	stakeholders={[
		{
			name: "Sohaib Ahmed",
			position: "Founder & CEO",
			bio: "Built &facts to give product teams the speed and certainty they need to win in competitive markets.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Sarah Kim",
			position: "Head of Data Science",
			bio: "Expert in consumer behavior analytics, transforming billions of data points into actionable insights.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Marcus Chen",
			position: "VP of Product",
			bio: "Former product manager who understands the validation challenges facing modern consumer brands.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<StakeholderGrid
	stakeholderType="investor"
	title="Backed by the best."
	subtitle="Point Nine, TSIC and others"
	stakeholders={[
		{
			name: "Point Nine Capital",
			image: "https://cdn.brandfetch.io/pointnine.com/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7"
		},
		{
			name: "TSIC Ventures",
			image: "https://cdn.brandfetch.io/tiny.vc/w/400/h/400/logo?c=1a2b3c4d5e"
		},
		{
			name: "Sequoia Capital",
			image: "https://cdn.brandfetch.io/sequoiacap.com/w/400/h/400/logo"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to move faster?"
	subtitle="Get instant market validation"
	description="Join the fast-growing consumer brands already using &facts to validate product concepts and make data-backed decisions in minutes, not weeks."
/>
