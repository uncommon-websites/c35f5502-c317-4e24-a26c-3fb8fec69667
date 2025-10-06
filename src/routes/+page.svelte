<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";

	// Icons
	import IconZap from "~icons/lucide/zap";
	import IconTarget from "~icons/lucide/target";
	import IconBrain from "~icons/lucide/brain";
	import IconShield from "~icons/lucide/shield-check";
	import IconTrendingUp from "~icons/lucide/trending-up";
	import IconFileCheck from "~icons/lucide/file-check";
</script>

<Hero
	centered={false}
	title="Get your grants approved in hours, not months"
	subtitle="Transform complex SR&ED applications into automated three-hour processes. Zero Draft AI eliminates consultant dependency and captures non-dilutive funding for Canadian tech companies."
	imageSrc="/generated/image-a-canadian-founder-sits-at-a-modern-offi.webp"
	callsToAction={[
		{
			href: "/contact",
			label: "Start your application"
		},
		{
			href: "/about",
			label: "See how it works"
		}
	]}
/>
<LogoScroller
	label="Trusted by innovative Canadian companies"
	logoUrls={[
		'https://cdn.brandfetch.io/shopify.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/wealthsimple.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/notion.so/w/400/h/400/logo',
		'https://cdn.brandfetch.io/hootsuite.com/w/400/h/400/logo'
	]}
/>

<Summary
	title="What we do"
	text="Zero Draft AI automates the entire grant application process for Canadian tech companies, transforming what typically takes months of consultant work into a three-hour automated workflow. We help growth-stage startups and SMBs secure SR&ED tax credits and other non-dilutive funding by handling the complex paperwork, identifying pre-qualified programs, and maximizing approval rates. Our platform eliminates the traditional bottlenecks of grant acquisition, allowing founders and CFOs to focus on building their business instead of navigating bureaucracy."
/>

<Testimonials
	testimonials={[
		{
			name: "Priya Mehta",
			position: "CFO",
			company: "VeloTech Systems",
			quote:
				"We recovered $340K in SR&ED credits in just three hours. Zero Draft eliminated the need for expensive consultants and gave us complete visibility into our application status. The automated process caught eligible expenses our previous consultant missed.",
			image: "/generated/image-a-south-asian-woman-poised-and-content-i.webp"
		},
		{
			name: "Marcus Chen",
			position: "Founder & CEO",
			company: "Quantum Labs",
			quote:
				"Instead of spending six weeks compiling documentation, our R&D team submitted our SR&ED claim in an afternoon. Zero Draft's AI identified $180K in qualifying activities we didn't even know were eligible. The approval came back in record time.",
			image: "/generated/image-a-confident-black-man-in-smart-modern-bu.webp"
		},
		{
			name: "Jennifer Park",
			position: "VP of Engineering",
			company: "DataFlow Analytics",
			quote:
				"Zero Draft found us eight pre-qualified grant programs beyond SR&ED, securing an additional $520K in non-dilutive funding. What used to take our team months now happens automatically. The risk assessment feature gave us confidence before we even applied.",
			image: "/generated/image-a-confident-asian-woman-in-business-atti.webp"
		}
	]}
/>

<Features
	title="Built for speed, designed for success"
	subtitle="Everything you need to secure non-dilutive funding without the consultant fees or months-long wait times"
	features={[
		{
			title: "Three-hour applications",
			description:
				"Complete SR&ED tax credit applications in hours instead of months. Our AI handles the entire workflow end-to-end while you focus on building your business.",
			icon: IconZap
		},
		{
			title: "Pre-qualified program matching",
			description:
				"Automatically discover and apply to dozens of grant programs where you're likely to succeed. We identify opportunities you didn't know existed.",
			icon: IconTarget
		},
		{
			title: "Intelligent document generation",
			description:
				"AI-powered automation transforms technical details into grant-ready applications. No more wrestling with complex paperwork or consultant dependencies.",
			icon: IconBrain
		},
		{
			title: "Maximized approval rates",
			description:
				"Our platform overcomes skepticism about grant success by applying proven strategies that increase your chances of approval across multiple programs.",
			icon: IconShield
		},
		{
			title: "Scale to thousands monthly",
			description:
				"Process unlimited applications simultaneously as your funding needs grow. Built to handle everything from single SR&ED credits to comprehensive grant portfolios.",
			icon: IconTrendingUp
		},
		{
			title: "End-to-end automation",
			description:
				"From eligibility assessment to final submission, every step is automated. Zero Draft eliminates the traditional bottlenecks of grant acquisition.",
			icon: IconFileCheck
		}
	]}
/>
<AboutTeaser />
<CallToAction
	title="Stop losing funding to complexity"
	subtitle="Start winning with automation"
	description="Canadian tech companies waste months navigating grant applications while competitors secure funding in hours. Zero Draft AI automatically identifies and applies to dozens of pre-qualified programs where you're likely to succeed. Get your SR&ED tax credits approved without consultant fees."
	imageSrc="/generated/image-a-canadian-business-founder-in-a-modern-.webp"
	callsToAction={[
		{
			href: "/contact",
			label: "Automate your first application",
			variant: "primary"
		},
		{
			href: "/about",
			label: "See approval rates",
			variant: "secondary"
		}
	]}
/>
