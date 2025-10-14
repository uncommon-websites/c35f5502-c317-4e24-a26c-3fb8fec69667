<!--
@component QualificationSection
A section that displays qualification criteria and value propositions.

Usage:
```html
<QualificationSection
  title="Built for Canadian innovators"
  qualifications={[...]}
  valueProps={[...]}
/>
```
-->
<script lang="ts">
	// Types
	import type { Component } from "svelte";

	type QualificationItem = {
		text: string;
	};

	type ValueProp = {
		title: string;
		description: string;
		icon?: Component;
	};

	// Props
	const {
		title,
		qualifications = [],
		valueProps = [],
		...rest
	}: {
		title: string;
		qualifications: QualificationItem[];
		valueProps: ValueProp[];
		[key: string]: any;
	} = $props();
</script>

<section class="bg-background" {...rest}>
	<div class="section-px section-py container mx-auto">
		<div class="mx-auto grid max-w-4xl gap-16">
			<!-- Title -->
			<h2 class="text-title1 text-center">{title}</h2>

			<!-- Qualifications -->
			<div class="grid gap-6">
				<p class="text-headline text-emphasis-low">If you're a Canadian business that:</p>
				<ul class="grid gap-4">
					{#each qualifications as item}
						<li class="text-headline flex items-start gap-3">
							<span class="text-primary mt-1">•</span>
							<span>{item.text}</span>
						</li>
					{/each}
				</ul>
				<p class="text-headline text-emphasis-low">
					Then you likely qualify, even if you've never applied before.
				</p>
			</div>

			<!-- Value Props -->
			<div class="grid gap-8 md:grid-cols-3">
				{#each valueProps as prop}
					<div class="grid gap-3">
						{#if prop.icon}
							{@const Icon = prop.icon}
							<Icon class="text-primary size-8" />
						{/if}
						<h3 class="text-title3">{prop.title}</h3>
						<p class="text-body text-emphasis-low">{prop.description}</p>
					</div>
				{/each}
			</div>
		</div>
	</div>
</section>
