<script>
	let openIndex = 0;
	const faqs = [
		{
			question: "Who is Auto Genius Speed Layer for?",
			answer: "Speed Layer is built for automotive dealership marketing directors who need faster websites but are losing sales to slow load times. We serve dealerships of all sizes, from single rooftops to large multi-location groups."
		},
		{
			question: "How long does implementation take?",
			answer: "Implementation is fast and simple. We integrate via a lightweight JavaScript tag that works with your existing CMS—no rebuild required. Most dealerships are live within days, with automated tagging requiring no IT lift from your team."
		},
		{
			question: "Will Speed Layer work with my current website platform?",
			answer: "Yes! Speed Layer works with all major automotive CMS platforms including Dealer.com, Dealer Inspire, WordPress, CDK, and many more. Our edge-computing technology sits on top of your existing infrastructure."
		},
		{
			question: "What if something goes wrong?",
			answer: "Speed Layer includes a built-in fail-safe that silently disables if any issues occur. Your website stays live and functional with zero risk to your dealership operations. We also provide continuous monitoring and weekly optimization updates."
		},
		{
			question: "How much does Speed Layer cost?",
			answer: "Retail pricing ranges from $1,300-$2,160 per month per rooftop. Stellantis dealers receive preferred pricing, and we offer group discounts for 5+ rooftops. This is more cost-effective than boosting SEM budgets 34% to achieve equivalent conversion lift."
		},
		{
			question: "What kind of results can I expect?",
			answer: "Dealerships typically see 3.2s average load time improvement, 34% conversion lift, and significant PageSpeed score increases. We provide structured reporting at T+7 days, monthly, and end-of-pilot with full analytics including engagement rate, bounce rate, and lead lifts."
		}
	];
</script>

<section class="py-24 bg-white">
	<div class="mx-auto max-w-[1400px] px-6">
		<div class="grid grid-cols-1 gap-16 lg:grid-cols-12">
			<!-- Left Side -->
			<div class="lg:col-span-4">
				<div class="mb-4 text-[10px] font-bold tracking-widest text-gray-500 uppercase">[06] FAQ</div>
				<h2 class="mb-6 text-4xl font-bold tracking-tight text-gray-950">Your questions, answered</h2>
				<p class="mb-8 text-lg leading-relaxed text-gray-600">
					We're here to help. Reach out to our team for guidance on how Speed Layer can accelerate your dealership website and increase conversions.
				</p>
				<a href="#" class="inline-block bg-gray-950 px-6 py-3 text-[11px] font-bold tracking-widest text-primary-400 transition-colors hover:bg-gray-900 uppercase">
					Book a Demo
				</a>
			</div>

			<!-- Right Side (Accordion) -->
			<div class="lg:col-span-8">
				<div class="divide-y divide-gray-200 border-t border-b border-gray-200">
					{#each faqs as faq, i}
						<div class="group">
							<button 
								class="flex w-full items-center justify-between py-6 text-left focus:outline-none"
								onclick={() => openIndex = openIndex === i ? -1 : i}
							>
								<span class="text-lg font-medium text-gray-900">{faq.question}</span>
								<span class="ml-4 flex h-6 w-6 items-center justify-center text-gray-400">
									{#if openIndex === i}
										<svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 6L6 18M6 6l12 12"/></svg>
									{:else}
										<svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 5v14M5 12h14"/></svg>
									{/if}
								</span>
							</button>
							{#if openIndex === i}
								<div class="pb-6 text-gray-600 leading-relaxed">
									{faq.answer}
								</div>
							{/if}
						</div>
					{/each}
				</div>
			</div>
		</div>
	</div>
</section>