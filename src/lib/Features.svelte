<script lang="ts">
	import { Users, TrendingUp, Building2 } from 'lucide-svelte';
</script>

<section class="max-w-[1200px] mx-auto px-6 py-20">
	<div class="mb-16 text-center max-w-3xl mx-auto">
		<h2 class="text-4xl font-serif text-gray-900 mb-6">
			Built for how brokers work
		</h2>
		<p class="text-xl text-gray-500">
			Stop juggling spreadsheets, email threads, and disconnected tools. Renlo brings everything together in one intelligent system.
		</p>
	</div>

	<!-- Grid of three benefits -->
	<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
		<!-- Unified relationships -->
		<div class="flex flex-col items-center text-center p-8 border border-gray-200 rounded-xl bg-white">
			<div class="w-20 h-20 mb-6 flex items-center justify-center relative">
				<!-- Abstract symbol for relationships -->
				<div class="absolute inset-0 flex items-center justify-center">
					<svg width="80" height="80" viewBox="0 0 80 80" fill="none">
						<!-- Three connected circles representing relationships -->
						<circle cx="40" cy="25" r="8" stroke="black" stroke-width="1.5" fill="none"/>
						<circle cx="25" cy="50" r="8" stroke="black" stroke-width="1.5" fill="none"/>
						<circle cx="55" cy="50" r="8" stroke="black" stroke-width="1.5" fill="none"/>
						<!-- Connecting lines -->
						<line x1="40" y1="33" x2="30" y2="44" stroke="black" stroke-width="1.5"/>
						<line x1="40" y1="33" x2="50" y2="44" stroke="black" stroke-width="1.5"/>
						<line x1="33" y1="50" x2="47" y2="50" stroke="black" stroke-width="1.5"/>
					</svg>
				</div>
			</div>
			<h3 class="text-xl font-bold text-gray-900 mb-4">Unified relationships</h3>
			<p class="text-gray-500 leading-relaxed">
				Every interaction, email, and meeting automatically tracked. Build deeper relationships with landlords, tenants, and investors.
			</p>
		</div>

		<!-- Deal intelligence -->
		<div class="flex flex-col items-center text-center p-8 border border-gray-200 rounded-xl bg-white">
			<div class="w-20 h-20 mb-6 flex items-center justify-center relative">
				<!-- Abstract symbol for deal flow -->
				<div class="absolute inset-0 flex items-center justify-center">
					<svg width="80" height="80" viewBox="0 0 80 80" fill="none">
						<!-- Ascending bars representing growth -->
						<rect x="15" y="50" width="12" height="15" stroke="black" stroke-width="1.5" fill="none"/>
						<rect x="34" y="40" width="12" height="25" stroke="black" stroke-width="1.5" fill="none"/>
						<rect x="53" y="25" width="12" height="40" stroke="black" stroke-width="1.5" fill="none"/>
						<!-- Upward arrow -->
						<path d="M 60 18 L 60 25 M 60 18 L 56 22 M 60 18 L 64 22" stroke="black" stroke-width="1.5"/>
					</svg>
				</div>
			</div>
			<h3 class="text-xl font-bold text-gray-900 mb-4">Deal intelligence</h3>
			<p class="text-gray-500 leading-relaxed">
				Track every deal from first contact to close. See your entire pipeline at a glance with real-time updates and smart insights.
			</p>
		</div>

		<!-- Property tracking -->
		<div class="flex flex-col items-center text-center p-8 border border-gray-200 rounded-xl bg-white">
			<div class="w-20 h-20 mb-6 flex items-center justify-center relative">
				<!-- Abstract symbol for property -->
				<div class="absolute inset-0 flex items-center justify-center">
					<svg width="80" height="80" viewBox="0 0 80 80" fill="none">
						<!-- Building outline -->
						<rect x="25" y="30" width="30" height="35" stroke="black" stroke-width="1.5" fill="none"/>
						<!-- Roof -->
						<path d="M 20 30 L 40 15 L 60 30" stroke="black" stroke-width="1.5" fill="none"/>
						<!-- Windows -->
						<rect x="30" y="38" width="6" height="6" stroke="black" stroke-width="1"/>
						<rect x="44" y="38" width="6" height="6" stroke="black" stroke-width="1"/>
						<rect x="30" y="50" width="6" height="6" stroke="black" stroke-width="1"/>
						<rect x="44" y="50" width="6" height="6" stroke="black" stroke-width="1"/>
					</svg>
				</div>
			</div>
			<h3 class="text-xl font-bold text-gray-900 mb-4">Property tracking</h3>
			<p class="text-gray-500 leading-relaxed">
				Centralize property data, market comps, and listing details. Everything you need to move deals forward in one place.
			</p>
		</div>
	</div>
</section>
