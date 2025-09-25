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
	title="Own your audience, not just your reach"
	subtitle="Freequency gives you full control of fan relationships by turning fragmented user activity into growth-ready identities—no blockchain experience needed."
	imageSrc="/generated/image-a-softly-lit-interior-wall-painted-in-ge.webp"
/>
<LogoScroller 
	label="Trusted by industry leaders"
	logoUrls={[
		'https://cdn.brandfetch.io/riot.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/espn.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/draftkings.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/twitch.tv/w/400/h/400/logo'
	]}
/>

<Summary
	title="What we do"
	text="Freequency transforms how brands connect with their audiences by unifying fragmented user data into direct, owned relationships. We help growth marketing teams at gaming studios, sports leagues, and consumer brands reduce platform dependency while turning every user interaction into acquisition fuel. Our plug-and-play Web3 infrastructure requires zero blockchain knowledge—just plug in and watch your audience ownership grow."
/>

<Testimonials
	testimonials={[
		{
			name: "Maya Chen",
			position: "VP of Growth Marketing",
			company: "Nexus Gaming",
			quote:
				"Freequency cut our customer acquisition costs by 60% within six months. Instead of chasing audiences across fragmented platforms, we now own direct relationships with over 2 million gamers. The SDK integration took our team just two days—no blockchain expertise needed.",
			image: "/generated/image-professional-headshot-of-an-asian-americ.webp"
		},
		{
			name: "Marcus Thompson",
			position: "Head of Fan Engagement",
			company: "Thunder Sports League",
			quote:
				"Before Freequency, we were losing 40% of our fan data to platform changes and iOS updates. Now we have unified fan identities that generated $3.2M in direct revenue last quarter alone. The risk of depending on third-party platforms is completely eliminated.",
			image: "/generated/image-professional-headshot-of-a-black-male-in.webp"
		},
		{
			name: "Sofia Rodriguez",
			position: "Chief Marketing Officer",
			company: "Arena Entertainment",
			quote:
				"What used to take our team 3 weeks to launch—coordinating campaigns across Discord, social media, and our app—now takes 3 days with Freequency's unified system. We've saved over 200 hours monthly while doubling our engagement rates. It's like having a growth team that never sleeps.",
			image: "/generated/image-professional-headshot-of-a-latina-female.webp"
		}
	]}
/>

<Features
	title="Built for brands, not blockchain"
	subtitle="Transform fragmented user interactions into direct audience ownership with infrastructure that just works"
	features={[
		{
			title: "Direct audience ownership",
			description: "Turn platform-dependent followers into owned relationships with unified cross-platform fan identities that eliminate dependency on external algorithms."
		},
		{
			title: "Zero blockchain complexity",
			description: "Plug-and-play SDK integration requires no Web3 knowledge—your team can implement sophisticated blockchain infrastructure in minutes, not months."
		},
		{
			title: "Unified data intelligence",
			description: "Consolidate fragmented user data across channels into actionable insights with AI-driven personalization that reduces acquisition costs by up to 40%."
		},
		{
			title: "Growth-ready identities",
			description: "Convert every user interaction into acquisition fuel with persistent identities that compound engagement and drive sustainable growth across your ecosystem."
		},
		{
			title: "Familiar user experiences",
			description: "Deliver Web3 benefits through interfaces your users already understand, eliminating friction while building deeper brand loyalty and community engagement."
		},
		{
			title: "Proof of Liquidity infrastructure",
			description: "Built on Berachain's innovative consensus mechanism, our EVM-compatible platform ensures scalable, cost-effective transactions that grow with your audience."
		}
	]}
/>
<AboutTeaser />
<CallToAction 
	title="Start owning your growth"
	subtitle="Acquisition costs are rising while platforms keep more of your data"
	description="Freequency helps you reduce customer acquisition costs by turning fragmented user data into direct, owned relationships. Get plug-and-play Web3 infrastructure that requires zero blockchain knowledge—just plug in and watch your audience ownership grow."
	imageSrc="/generated/image-a-professional-growth-marketing-director.webp"
	callsToAction={[
		{
			href: "/contact",
			label: "Book a live demo",
			variant: "primary"
		},
		{
			href: "/get-started",
			label: "Get started free",
			variant: "secondary"
		}
	]}
/>
