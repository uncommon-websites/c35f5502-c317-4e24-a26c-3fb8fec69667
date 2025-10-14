<!--
@component FAQ
A component to display frequently asked questions.

Usage:
```html
<FAQ
  title="Frequently asked questions"
  faqs={[
    { question: "...", answer: "..." }
  ]}
/>
```
-->
<script lang="ts">
	// Types
	type FAQItem = {
		question: string;
		answer: string;
	};

	// Props
	const {
		title = "Frequently asked questions",
		faqs = [],
		...rest
	}: {
		title?: string;
		faqs: FAQItem[];
		[key: string]: any;
	} = $props();

	// State for accordion
	let openIndex = $state<number | null>(null);

	function toggleFAQ(index: number) {
		openIndex = openIndex === index ? null : index;
	}
</script>

<section class="bg-background" {...rest}>
	<div class="section-px section-py container mx-auto">
		<div class="mx-auto grid max-w-3xl gap-12">
			<!-- Title -->
			<h2 class="text-title1 text-center">{title}</h2>

			<!-- FAQ Items -->
			<div class="grid gap-4">
				{#each faqs as faq, index}
					<div class="bg-card border-border rounded-(--radius) border">
						<button
							class="text-title3 flex w-full items-center justify-between gap-4 p-6 text-left transition-colors hover:bg-muted/50"
							onclick={() => toggleFAQ(index)}
							aria-expanded={openIndex === index}
						>
							<span>{faq.question}</span>
							<span
								class="text-emphasis-low shrink-0 transition-transform duration-200"
								class:rotate-180={openIndex === index}
							>
								<svg
									xmlns="http://www.w3.org/2000/svg"
									width="24"
									height="24"
									viewBox="0 0 24 24"
									fill="none"
									stroke="currentColor"
									stroke-width="2"
									stroke-linecap="round"
									stroke-linejoin="round"
								>
									<path d="m6 9 6 6 6-6" />
								</svg>
							</span>
						</button>
						{#if openIndex === index}
							<div class="text-body text-emphasis-low border-t border-border p-6 pt-4">
								{faq.answer}
							</div>
						{/if}
					</div>
				{/each}
			</div>
		</div>
	</div>
</section>
