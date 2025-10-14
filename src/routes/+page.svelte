<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
	import QualificationSection from "$lib/components/layout/QualificationSection.svelte";
	import CaseStudy from "$lib/components/layout/CaseStudy.svelte";
	import HowItWorks from "$lib/components/layout/HowItWorks.svelte";
	import FAQ from "$lib/components/layout/FAQ.svelte";

	// Icons
	import IconClock from "~icons/lucide/clock";
	import IconShieldCheck from "~icons/lucide/shield-check";
	import IconDollarSign from "~icons/lucide/dollar-sign";
</script>

<Hero
	centered={false}
	title="Claim millions in SR&ED faster than ever"
	subtitle="Audit-ready claims. White-glove service. Trusted by enterprise finance teams."
	imageSrc="/generated/image-a-canadian-founder-sits-at-a-modern-offi.webp"
	callsToAction={[
		{
			href: "/contact",
			label: "Book my free assessment"
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
	title="SR&ED in two hours, not eighty"
	text="ZeroDraft helps Canadian enterprises unlock millions in non-dilutive funding without bottlenecks, wasted time, or compliance risk that normally come with filing. Every claim is produced faster, more accurately, and fully audit-ready. Our licensed CPAs and engineers review every submission, maintaining one of the highest success rates in the industry."
/>

<QualificationSection
	title="Built for Canadian innovators"
	qualifications={[
		{ text: "Has salaried technical staff" },
		{ text: "Develops new products, software, or IP" },
		{ text: "Is incorporated and pays taxes in Canada" }
	]}
	valueProps={[
		{
			title: "Save weeks of effort",
			description: "Your team spends less than 2 hours on a claim that can yield $500K+ in tax credits.",
			icon: IconClock
		},
		{
			title: "Accuracy you can trust",
			description: "Every claim is validated by our licensed CPAs to ensure it's audit-ready.",
			icon: IconShieldCheck
		},
		{
			title: "No bloated 15%+ fees",
			description: "We don't charge inflated 15%+ commissions like traditional SR&ED consultants.",
			icon: IconDollarSign
		}
	]}
/>

<Testimonials
	testimonials={[
		{
			name: "Jason T.",
			position: "CEO",
			company: "AgriCore",
			quote:
				"We used to spend 40+ hours writing grants. With ZeroDraft, we got $120K back in 6 days—with barely any time invested.",
			image: "/generated/image-a-confident-black-man-in-smart-modern-bu.webp"
		},
		{
			name: "Priya N.",
			position: "CTO",
			company: "Cannabis Tech Startup",
			quote:
				"I thought we wouldn't qualify. Turns out we were eligible for three different programs. The process was smoother than I imagined.",
			image: "/generated/image-a-south-asian-woman-poised-and-content-i.webp"
		}
	]}
/>

<section class="bg-background">
	<div class="section-px section-py container mx-auto">
		<div class="mx-auto grid max-w-4xl gap-12 text-center">
			<div class="grid gap-6">
				<h2 class="text-title1">Why ZeroDraft is the fastest path to SR&ED success</h2>
				<div class="text-headline text-emphasis-low mx-auto max-w-3xl space-y-4">
					<p>
						When your SR&ED process runs the way it should, everything moves faster. You scale with
						confidence, hire without hesitation, and stop guessing when funding will land. Filing
						becomes a formality, not an annual disruption.
					</p>
					<p>
						But when it doesn't work? You don't just lose money. You risk a CRA audit and potential
						blacklisting from the SR&ED program.
					</p>
				</div>
			</div>
			<a
				href="/contact"
				class="bg-primary text-primary-foreground hover:bg-primary/90 mx-auto inline-flex items-center justify-center rounded-(--radius) px-8 py-3 text-callout transition-colors"
			>
				Book my free assessment
			</a>
		</div>
	</div>
</section>

<CaseStudy
	title="How SearchEye recovered $190,000 after a rejection"
	description="When SearchEye's initial SR&ED claim was outright rejected, it triggered a full CRA audit. Weeks of stress, 30+ hours of document requests, and a major operational distraction. We stepped in, rebuilt their claim from the ground up, and got them approved with $190,000 with less than five hours of work from their team."
	result="$190,000"
	cta={{ href: "/contact", label: "See how we did it" }}
	imageSrc="/generated/image-a-diverse-professional-business-team-in-.webp"
/>

<HowItWorks
	title="Transparent. Efficient. Proven."
	subtitle="We built the most cost-effective SR&ED process in the industry, powered by automation and CPA oversight. No inflated commissions, and no hidden costs. Just faster, audit-ready claims. Here's how it works:"
	steps={[
		{
			number: 1,
			title: "You tell us about your business on a 15-min call"
		},
		{
			number: 2,
			title: "Our platform + CPA experts provide audit-ready documentation"
		},
		{
			number: 3,
			title: "You submit your claim"
		}
	]}
	guarantee="Guaranteed timeline: 5 days from intake to filing"
/>
<FAQ
	faqs={[
		{
			question: "How much can I get?",
			answer: "$500K+ depending on your business and scope of R&D."
		},
		{
			question: "Do I need technical documentation?",
			answer: "No. Our engineers will extract the details needed to submit a compliant claim."
		},
		{
			question: "What if I've already applied in the past?",
			answer: "We'll review your past claims and may be able to find missed opportunities."
		},
		{
			question: "Is my information secure?",
			answer: "Yes. We use bank-level encryption and secure data storage protocols to protect your financial and technical data."
		},
		{
			question: "Who has access to my data?",
			answer: "Only our vetted CPAs. We never outsource to unauthorized third parties."
		},
		{
			question: "Is your documentation audit-proof?",
			answer: "Yes. Every claim is prepared with CRA guidelines in mind and reviewed by licensed professionals."
		},
		{
			question: "Have your claims ever been rejected?",
			answer: "We maintain a high success rate. If there's an issue, we'll revise and resubmit at no cost to you."
		}
	]}
/>

<CallToAction
	title="It's your money"
	subtitle="Don't leave it on the table"
	description="Reduce filing time by more than 95 percent, improve compliance, and recover millions in non-dilutive funding without tying up your team for months."
	imageSrc="/generated/image-a-canadian-business-founder-in-a-modern-.webp"
	callsToAction={[
		{
			href: "/contact",
			label: "Book my free consultation now",
			variant: "primary"
		}
	]}
/>
