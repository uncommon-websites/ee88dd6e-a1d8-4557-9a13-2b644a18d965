<script lang="ts">
</script>

<section class="pt-24 pb-32 px-6 max-w-[1200px] mx-auto relative">
	<!-- Background gradient effect that fades out -->
	<div class="absolute inset-0 -mx-[100vw] pointer-events-none overflow-hidden">
		<div class="absolute inset-0 bg-gradient-to-b from-gray-50 via-gray-50/40 to-transparent"></div>
	</div>
	
	<!-- Patterned background that fades out -->
	<div class="absolute bottom-0 left-0 right-0 h-48 pointer-events-none">
		<div class="absolute inset-0 opacity-[0.03]">
			<svg width="100%" height="100%" xmlns="http://www.w3.org/2000/svg">
				<defs>
					<pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
						<path d="M 40 0 L 0 0 0 40" fill="none" stroke="black" stroke-width="1"/>
					</pattern>
					<linearGradient id="fade" x1="0%" y1="0%" x2="0%" y2="100%">
						<stop offset="0%" style="stop-color:black;stop-opacity:1" />
						<stop offset="100%" style="stop-color:black;stop-opacity:0" />
					</linearGradient>
					<mask id="fademask">
						<rect width="100%" height="100%" fill="url(#fade)"/>
					</mask>
				</defs>
				<rect width="100%" height="100%" fill="url(#grid)" mask="url(#fademask)"/>
			</svg>
		</div>
	</div>
	<div class="flex flex-col lg:flex-row items-center gap-12 lg:gap-16">
		<!-- Text Content -->
		<div class="flex-1 text-center lg:text-left">
			<div class="inline-flex items-center gap-2 text-xs font-medium text-gray-500 mb-8 border border-gray-200 rounded-full px-3 py-1 bg-white">
				<span class="w-2 h-2 bg-green-500 rounded-full animate-pulse"></span>
				In Limited Early Access
			</div>

			<h1 class="text-[56px] leading-[1.1] font-serif tracking-tight text-gray-900 mb-6">
				The Modern OS for High-Performance Brokers
			</h1>

			<p class="text-lg text-gray-500 mb-10 max-w-xl text-balance lg:mx-0 mx-auto">
				Renlo replaces fragmented CRMs and deal trackers with a single system built around how CRE deals really happen.
			</p>

			<div class="flex items-center justify-center lg:justify-start gap-4">
				<a href="#" class="bg-black text-white text-sm font-medium px-5 py-2.5 rounded-lg hover:bg-gray-800 transition-colors">
					Book a call
				</a>
			</div>
		</div>

		<!-- Abstract Animated Element -->
		<div class="flex-shrink-0 w-[280px] h-[280px] relative">
			<!-- Rotating outer ring -->
			<div class="absolute inset-0 border-2 border-gray-200 rounded-full animate-[spin_20s_linear_infinite]"></div>
			
			<!-- Pulsing middle ring -->
			<div class="absolute inset-8 border-2 border-gray-300 rounded-full animate-[spin_15s_linear_infinite_reverse] opacity-60"></div>
			
			<!-- Inner rotating dots -->
			<div class="absolute inset-16 animate-[spin_10s_linear_infinite]">
				<div class="absolute top-0 left-1/2 w-3 h-3 bg-black rounded-full -translate-x-1/2"></div>
				<div class="absolute bottom-0 left-1/2 w-3 h-3 bg-gray-400 rounded-full -translate-x-1/2"></div>
				<div class="absolute left-0 top-1/2 w-3 h-3 bg-gray-600 rounded-full -translate-y-1/2"></div>
				<div class="absolute right-0 top-1/2 w-3 h-3 bg-gray-300 rounded-full -translate-y-1/2"></div>
			</div>
			
			<!-- Center pulsing core -->
			<div class="absolute inset-0 flex items-center justify-center">
				<div class="w-12 h-12 bg-black rounded-full animate-pulse"></div>
			</div>
			
			<!-- Connecting lines -->
			<svg class="absolute inset-0 w-full h-full animate-[spin_25s_linear_infinite]" viewBox="0 0 280 280">
				<line x1="140" y1="40" x2="140" y2="100" stroke="currentColor" stroke-width="1" class="text-gray-200" />
				<line x1="140" y1="180" x2="140" y2="240" stroke="currentColor" stroke-width="1" class="text-gray-200" />
				<line x1="40" y1="140" x2="100" y2="140" stroke="currentColor" stroke-width="1" class="text-gray-200" />
				<line x1="180" y1="140" x2="240" y2="140" stroke="currentColor" stroke-width="1" class="text-gray-200" />
			</svg>
		</div>
	</div>
</section>

<style>
	@keyframes spin {
		from {
			transform: rotate(0deg);
		}
		to {
			transform: rotate(360deg);
		}
	}
</style>
