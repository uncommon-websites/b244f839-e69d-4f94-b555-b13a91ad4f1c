<script>
	// Navbar
</script>

<div class="sticky top-0 z-50 w-full bg-white">
	<!-- Top Banner -->
	<div class="bg-gray-950 px-4 py-2 text-center text-[11px] font-medium tracking-wide text-white">
		<a href="#" class="hover:underline">
			Stellantis Partnership: Preferred pricing for all dealerships &rarr; Learn More
		</a>
	</div>

	<!-- Main Navigation -->
	<nav class="border-b border-gray-200 px-6 py-4">
		<div class="mx-auto flex max-w-[1400px] items-center justify-between">
			<!-- Logo and Left Links -->
			<div class="flex items-center gap-12">
				<a href="/" class="flex items-center gap-2">
					<svg width="24" height="52" viewBox="0 0 567 1238" fill="none" xmlns="http://www.w3.org/2000/svg">
						<g clip-path="url(#clip0_4854_2)">
							<path d="M528.434 579.434H283.4V0H243.847L2.76704 605.746C-7.31911 631.068 11.271 658.566 38.563 658.566H283.596V1238H323.151L564.426 632.254C574.514 606.932 555.924 579.434 528.632 579.434H528.434Z" fill="black"/>
						</g>
						<defs>
							<clipPath id="clip0_4854_2">
								<rect width="567" height="1238" fill="white"/>
							</clipPath>
						</defs>
					</svg>
					<span class="text-xl font-bold tracking-tight text-gray-900">Auto Genius</span>
				</a>
				
				<div class="hidden items-center gap-8 md:flex">
					{#each ['Speed Layer', 'Pricing', 'Resources', 'Case Studies'] as item}
						<a href="#" class="flex items-center gap-1 text-[11px] font-semibold tracking-widest text-gray-600 hover:text-gray-900 uppercase">
							{item}
							{#if item === 'Speed Layer' || item === 'Resources'}
								<svg width="10" height="10" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="opacity-50"><path d="m6 9 6 6 6-6"/></svg>
							{/if}
						</a>
					{/each}
				</div>
			</div>

			<!-- Right Actions -->
			<div class="flex items-center gap-6">
				<a href="#" class="text-[11px] font-semibold tracking-widest text-gray-600 hover:text-gray-900 uppercase">
					Community
				</a>
				<a href="#" class="text-[11px] font-semibold tracking-widest text-gray-600 hover:text-gray-900 uppercase">
					Book a Demo
				</a>
				<a href="#" class="bg-gray-950 px-4 py-2 text-[11px] font-bold tracking-widest text-primary-400 transition-colors hover:bg-gray-900 uppercase">
					Get Started
				</a>
			</div>
		</div>
	</nav>
</div>