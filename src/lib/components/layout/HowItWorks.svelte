<!--
@component HowItWorks
A component to display a step-by-step process.

Usage:
```html
<HowItWorks
  title="Transparent. Efficient. Proven."
  subtitle="..."
  steps={[...]}
  guarantee="Guaranteed timeline: 5 days from intake to filing"
/>
```
-->
<script lang="ts">
	// Types
	type Step = {
		number: number;
		title: string;
		description?: string;
	};

	// Props
	const {
		title,
		subtitle,
		steps = [],
		guarantee,
		...rest
	}: {
		title: string;
		subtitle: string;
		steps: Step[];
		guarantee?: string;
		[key: string]: any;
	} = $props();
</script>

<section class="bg-background" {...rest}>
	<div class="section-px section-py container mx-auto">
		<div class="mx-auto grid max-w-4xl gap-16">
			<!-- Header -->
			<div class="grid gap-4 text-center">
				<h2 class="text-title1">{title}</h2>
				<p class="text-headline text-emphasis-low mx-auto max-w-2xl">{subtitle}</p>
			</div>

			<!-- Steps -->
			<div class="grid gap-8">
				{#each steps as step}
					<div class="flex gap-6">
						<div
							class="bg-primary text-primary-foreground flex size-12 shrink-0 items-center justify-center rounded-full"
						>
							<span class="text-title3">{step.number}</span>
						</div>
						<div class="grid gap-2 pt-2">
							<h3 class="text-title3">{step.title}</h3>
							{#if step.description}
								<p class="text-body text-emphasis-low">{step.description}</p>
							{/if}
						</div>
					</div>
				{/each}
			</div>

			<!-- Guarantee -->
			{#if guarantee}
				<div class="bg-card border-border rounded-(--radius) border p-6 text-center">
					<p class="text-headline text-primary">{guarantee}</p>
				</div>
			{/if}
		</div>
	</div>
</section>
