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
			title: "Built for brands, not blockchain",
			description: "We emphasize practical utility over technical complexity, making Web3 accessible without requiring any blockchain knowledge."
		},
		{
			title: "Mission-driven empowerment",
			description: "Returning control to the people driving growth, we focus on empowering brands with direct audience ownership instead of platform dependency."
		},
		{
			title: "Innovation with purpose",
			description: "Disrupting the status quo by transforming fragmented user relationships into owned, unified identities that fuel sustainable growth."
		},
		{
			title: "Community-first approach",
			description: "Building lasting relationships through our plug-and-play ecosystem that turns every user interaction into acquisition fuel and competitive advantage."
		}
	];
</script>

<SecondaryHero
	title="Own your audience"
	subtitle="Growth without gatekeepers"
	imageSrc="/generated/image-a-modern-team-of-diverse-professionals-c.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Growth marketing teams face an impossible choice: pay rising acquisition costs to platforms that own your audience, or watch sustainable growth slip away. While brands pour millions into Facebook and Google ads, they're left with fragmented data and rented relationships that disappear the moment they stop paying. The digital advertising landscape has become a trap where success breeds dependency.",
		"Freequency breaks this cycle by transforming Web3 infrastructure into familiar user experiences that actually work for consumer brands. Our plug-and-play SDKs give growth teams blockchain-powered audience ownership without requiring any Web3 expertise. From gaming studios to sports leagues, brands can finally capture every fan interaction—on-chain and off—into a unified identity system that turns user activity into sustainable acquisition fuel.",
		"We're building a future where brands don't chase audiences but connect with them directly through owned relationships and first-party data. With Freequency, every Discord chat, in-game decision, and community interaction becomes part of a persistent user passport that powers cross-platform growth. This isn't just another marketing tool—it's the infrastructure that gives control back to the people actually driving digital progress."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<StakeholderGrid
	stakeholderType="investor"
	title="Powered by leading infrastructure"
	subtitle="Strategic partnership driving Web3 accessibility"
	stakeholders={[
		{
			name: "Berachain",
			position: "Primary L1 Partner",
			image: "https://logo.clearbit.com/berachain.com"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to build direct relationships?"
	subtitle="Growth without gatekeepers"
	description="Join forward-thinking brands using Freequency to transform fragmented user data into unified audience ownership. No blockchain expertise required—just plug-and-play SDKs that turn every interaction into sustainable acquisition fuel."
	imageSrc="/generated/image-a-professional-growth-marketing-director.webp"
/>
