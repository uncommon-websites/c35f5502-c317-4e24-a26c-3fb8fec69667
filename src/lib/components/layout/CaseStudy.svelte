<!--
@component CaseStudy
A component to display a case study with results and CTA.

Usage:
```html
<CaseStudy
  title="How SearchEye recovered $190,000 after a rejection"
  description="..."
  result="$190,000"
  cta={{ href: "/case-study", label: "See how we did it" }}
/>
```
-->
<script lang="ts">
	// Components
	import Button from "../ui/Button.svelte";

	// Types
	type CTA = {
		href: string;
		label: string;
	};

	// Props
	const {
		title,
		description,
		result,
		cta,
		imageSrc,
		...rest
	}: {
		title: string;
		description: string;
		result: string;
		cta: CTA;
		imageSrc?: string;
		[key: string]: any;
	} = $props();
</script>

<section class="bg-card" {...rest}>
	<div class="section-px section-py container mx-auto">
		<div class="mx-auto grid max-w-5xl gap-12 lg:grid-cols-2 lg:items-center">
			<!-- Content -->
			<div class="grid gap-8">
				<div class="grid gap-4">
					<h2 class="text-title2">{title}</h2>
					<p class="text-headline text-emphasis-low">{description}</p>
				</div>
				
				<!-- Result Highlight -->
				<div class="bg-background border-border grid gap-2 rounded-(--radius) border p-6">
					<p class="text-caption text-emphasis-low">Total recovered</p>
					<p class="text-display text-primary">{result}</p>
				</div>

				<Button href={cta.href} variant="primary" size="lg" class="w-fit">
					{cta.label}
				</Button>
			</div>

			<!-- Image -->
			{#if imageSrc}
				<div class="aspect-square overflow-hidden rounded-(--radius)">
					<img src={imageSrc} alt="Case study" class="size-full object-cover" />
				</div>
			{/if}
		</div>
	</div>
</section>
