<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CenteredTextOnlyHero from "$lib/components/layout/hero-sections/CenteredTextOnlyHero.svelte";
</script>

<CenteredTextOnlyHero
	title="Know what your customers want—instantly"
	subtitle="Validate new product ideas in minutes using real-world behavior, not weeks of surveys or guesswork."
	imageSrc="/generated/image-a-cozy-caf-interior-with-wooden-tables-a.webp"
/>
<LogoScroller 
	label="Trusted by industry leaders"
	logoUrls={[
		'https://cdn.brandfetch.io/warbyparker.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/allbirds.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/glossier.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/casper.com/w/400/h/400/logo'
	]}
/>

<Summary
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	generating={true}
	testimonials={[
		{
			name: "Maya Chen",
			position: "Product Manager",
			company: "NovaCare",
			quote:
				"&facts saved us 6 weeks of market research for our wellness product launch. We validated our concept in 3 days instead of months, preventing a $200K investment in a concept that would have failed.",
			image: "/generated/image-professional-headshot-of-a-confident-asi.webp"
		},
		{
			name: "Marcus Williams",
			position: "Innovation Director",
			company: "EcoTech Solutions",
			quote:
				"Traditional focus groups would have cost us $50K and taken 8 weeks. &facts delivered deeper insights in minutes for a fraction of the cost, helping us pivot our sustainable packaging before wasting development resources.",
			image: "/generated/image-professional-headshot-of-a-confident-bla.webp"
		},
		{
			name: "Isabella Rodriguez",
			position: "CEO",
			company: "Bloom Beauty",
			quote:
				"Before &facts, we launched 2 products that flopped, costing us $500K. Now we validate every concept first—our last 4 launches exceeded projections by 40% because we knew exactly what customers wanted.",
			image: "/generated/image-professional-headshot-of-a-confident-his.webp"
		}
	]}
/>

<Features
	title="Know what the market really wants"
	subtitle="&facts turns billions of real-world consumer signals into instant product validation—so you can stop guessing and start growing."
	features={[
		{
			title: "Real-world behavior, not biased opinions",
			description:
				"Stop relying on slow, survey-based research. Our platform analyzes actual buying behavior, search trends, and online activity to tell you what people are doing—not just what they say."
		},
		{
			title: "Answers in minutes, not weeks",
			description:
				"Get fully automated market validation reports in under 10 minutes. No agencies. No recruiters. No waiting."
		},
		{
			title: "Track what's already taking off",
			description:
				"Spot emerging trends, competitor traction, and untapped demand with real-time consumer signal data."
		},
		{
			title: "Validate new product ideas before launch",
			description:
				"De-risk launches with clear evidence of real-world demand instead of relying on guesswork or expensive traditional research."
		},
		{
			title: "Justify roadmaps with confidence", 
			description:
				"Arm your team with data that backs every decision and moves faster than competitors stuck in analysis paralysis."
		},
		{
			title: "Spot gaps your competitors missed",
			description:
				"Identify product white space based on how consumers are behaving today, not outdated market reports from months ago."
		}
	]}
/>
<AboutTeaser />
<CallToAction />
