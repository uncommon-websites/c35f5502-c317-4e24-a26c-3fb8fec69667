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
			title: "User empowerment",
			description: "Returning control to the people driving growth, focusing on empowerment over dependency."
		},
		{
			title: "Built for brands",
			description: "Emphasizing practical utility over technical complexity, creating tools that actually work for consumer marketers."
		},
		{
			title: "Community-centric",
			description: "Building lasting relationships and turning user activity into acquisition fuel through direct connections."
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

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Built by growth experts"
	subtitle="Who understand the challenges you face"
	stakeholders={[
		{
			name: "Alex Rodriguez",
			position: "Founder & CEO",
			bio: "Former growth lead at gaming studios, experienced the pain of fragmented user data firsthand.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Sam Chen",
			position: "Head of Product",
			bio: "Ex-Meta growth engineer focused on building Web3 tools that feel like Web2 experiences.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Taylor Kim",
			position: "Chief Technology Officer",
			bio: "Blockchain infrastructure specialist making complex technology accessible to consumer brands.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<StakeholderGrid
	stakeholderType="investor"
	title="Strategic partnerships"
	subtitle="Powered by leading Web3 infrastructure"
	stakeholders={[
		{
			name: "Berachain",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Web3 Growth Partners",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Gaming Ventures",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to own your audience?"
	subtitle="Stop renting, start owning"
	description="Join the gaming studios and sports leagues already using Freequency to transform user activity into sustainable acquisition fuel."
/>
