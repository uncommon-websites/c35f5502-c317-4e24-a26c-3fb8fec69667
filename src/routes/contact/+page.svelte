<script lang="ts">
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
</script>

<Hero
	centered={true}
	title="Get started with Zero Draft AI"
	subtitle="Transform your grant applications from months-long consultant engagements into automated three-hour processes. Book a demo to see how we can help you secure non-dilutive funding."
	callsToAction={[
		{
			href: "/",
			label: "Back to home"
		}
	]}
/>

<div class="section-px section-py container mx-auto">
	<div class="mx-auto max-w-2xl">
		<div class="grid gap-8">
			<div class="grid gap-4">
				<h2 class="text-title2">Contact us</h2>
				<p class="text-body text-muted-foreground">
					Ready to automate your grant applications? Get in touch with our team to learn how Zero Draft AI can help you secure SR&ED tax credits and other government funding programs.
				</p>
			</div>

			<div class="grid gap-6">
				<div class="grid gap-2">
					<label for="name" class="text-body font-medium">Name</label>
					<input
						type="text"
						id="name"
						name="name"
						class="rounded-md border px-4 py-2"
						style="border-color: var(--color-border); background-color: var(--color-background);"
						placeholder="Your name"
					/>
				</div>

				<div class="grid gap-2">
					<label for="email" class="text-body font-medium">Email</label>
					<input
						type="email"
						id="email"
						name="email"
						class="rounded-md border px-4 py-2"
						style="border-color: var(--color-border); background-color: var(--color-background);"
						placeholder="your@email.com"
					/>
				</div>

				<div class="grid gap-2">
					<label for="company" class="text-body font-medium">Company</label>
					<input
						type="text"
						id="company"
						name="company"
						class="rounded-md border px-4 py-2"
						style="border-color: var(--color-border); background-color: var(--color-background);"
						placeholder="Your company name"
					/>
				</div>

				<div class="grid gap-2">
					<label for="message" class="text-body font-medium">Message</label>
					<textarea
						id="message"
						name="message"
						rows="5"
						class="rounded-md border px-4 py-2"
						style="border-color: var(--color-border); background-color: var(--color-background);"
						placeholder="Tell us about your grant application needs"
					></textarea>
				</div>

				<button
					type="submit"
					class="inline-flex items-center justify-center rounded-md px-5 py-2 font-semibold transition"
					style="background-color: var(--color-primary); color: var(--color-primary-foreground);"
				>
					Send message
				</button>
			</div>
		</div>
	</div>
</div>
