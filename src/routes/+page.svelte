<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
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
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	generating
	testimonials={[
		{
			name: "Jane Smith",
			position: "CTO",
			company: "Tech Innovations",
			quote:
				"Their cutting-edge automation boosted our productivity by 35%.\nThe intuitive interface reduced training time and improved team adoption.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "John Doe",
			position: "Director of Operations",
			company: "Global Solutions",
			quote:
				"Their robust security protocols gave us confidence in handling sensitive data.\nThe 24/7 support team resolved issues within hours, not days.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Sarah Johnson",
			position: "Product Manager",
			company: "Future Systems",
			quote:
				"The scalable platform grew seamlessly with our business needs.\nTheir customization options allowed us to tailor solutions perfectly to our workflows.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<Features
	generating
	title="Features"
	subtitle="Some features"
	features={[
		{
			title: "Streamlined Workflows",
			description:
				"Automate repetitive tasks and connect systems to improve productivity with our industry-leading 87% time savings."
		},
		{
			title: "Data Analysis",
			description:
				"Extract meaningful insights from your data with powerful analytical tools backed by proprietary AI algorithms that are 3x more accurate than competitors."
		},
		{
			title: "Secure Collaboration",
			description:
				"Work together seamlessly while maintaining strict data privacy standards with our zero-knowledge architecture and military-grade encryption."
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
