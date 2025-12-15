<script lang="ts">
	import { ArrowRight, Zap, Bot, Database, BarChart3, Mail, MessageSquare, Calendar, CheckCircle2, Search, Plus, MoreHorizontal, Briefcase, Building2 } from 'lucide-svelte';
</script>

<section class="max-w-[1200px] mx-auto px-6 py-20">
	<div class="mb-20 max-w-2xl">
		<h2 class="text-4xl font-serif text-gray-900 mb-6">
			Built for how brokers work. <span class="text-gray-500 font-sans text-xl font-normal block mt-4">Stop juggling spreadsheets, email threads, and disconnected tools. Renlo brings everything together in one intelligent system.</span>
		</h2>
	</div>

	<div class="border border-gray-200 rounded-xl overflow-hidden bg-white shadow-sm">
		<!-- Row 1: Unified relationships -->
		<div class="grid grid-cols-1 md:grid-cols-3 border-b border-gray-200">
			<div class="p-12 flex flex-col justify-between border-r border-gray-200">
				<div>
					<h3 class="text-xl font-bold text-gray-900 mb-4">Unified relationships</h3>
					<p class="text-gray-500 leading-relaxed mb-8">
						Every interaction, email, and meeting automatically tracked. Build deeper relationships with landlords, tenants, and investors.
					</p>
				</div>
			</div>
			<div class="col-span-2 bg-gray-50/50 p-12 flex items-center justify-center overflow-hidden relative">
				<!-- Contact Card Mockup -->
				<div class="relative w-full max-w-md">
					<div class="bg-white border border-gray-200 rounded-lg shadow-sm overflow-hidden">
						<div class="p-4 border-b border-gray-100">
							<div class="flex items-start gap-3">
								<div class="w-12 h-12 rounded-full bg-gray-200 overflow-hidden flex-shrink-0">
									<img src="https://i.pravatar.cc/150?u=broker1" alt="" class="w-full h-full object-cover"/>
								</div>
								<div class="flex-1">
									<h4 class="font-semibold text-gray-900">Michael Chen</h4>
									<p class="text-sm text-gray-500">Principal, Brookfield Properties</p>
									<div class="flex items-center gap-2 mt-2">
										<span class="px-2 py-0.5 bg-green-100 text-green-700 text-[10px] rounded-full">Active</span>
										<span class="text-xs text-gray-400">Last contact: 2 days ago</span>
									</div>
								</div>
							</div>
						</div>
						<div class="p-4 space-y-3 text-xs">
							<div class="flex items-center gap-2 text-gray-600">
								<Mail size={14} class="text-gray-400" />
								<span>m.chen@brookfield.com</span>
							</div>
							<div class="flex items-center gap-2 text-gray-600">
								<Calendar size={14} class="text-gray-400" />
								<span>Meeting scheduled: Tomorrow 2pm</span>
							</div>
							<div class="flex items-center gap-2 text-gray-600">
								<Briefcase size={14} class="text-gray-400" />
								<span>3 active deals • $12.5M pipeline</span>
							</div>
						</div>
					</div>
				</div>
				
				<!-- Decorative geometric shape -->
				<div class="absolute bottom-10 right-10 opacity-20">
					<svg width="100" height="100" viewBox="0 0 100 100" fill="none">
						<path d="M50 0L93.3013 25V75L50 100L6.69873 75V25L50 0Z" stroke="black" stroke-width="1"/>
						<path d="M50 0V50M93.3013 25L50 50M93.3013 75L50 50M50 100V50M6.69873 75L50 50M6.69873 25L50 50" stroke="black" stroke-width="1"/>
					</svg>
				</div>
			</div>
		</div>

		<!-- Row 2: Deal intelligence -->
		<div class="grid grid-cols-1 md:grid-cols-3 border-b border-gray-200">
			<div class="p-12 flex flex-col justify-between border-r border-gray-200">
				<div>
					<h3 class="text-xl font-bold text-gray-900 mb-4">Deal intelligence</h3>
					<p class="text-gray-500 leading-relaxed mb-8">
						Track every deal from first contact to close. See your entire pipeline at a glance with real-time updates and smart insights.
					</p>
				</div>
			</div>
			<div class="col-span-2 bg-gray-50/50 p-12 flex items-center justify-center relative">
				<div class="bg-white rounded-xl shadow-sm border border-gray-200 w-full max-w-lg overflow-hidden">
					<div class="p-4 border-b border-gray-100">
						<h4 class="font-semibold text-gray-900">Active Deals</h4>
					</div>
					<div class="p-4 space-y-3">
						<!-- Deal 1 -->
						<div class="flex items-center justify-between p-3 bg-gray-50 rounded-lg">
							<div class="flex-1">
								<div class="flex items-center gap-2 mb-1">
									<Building2 size={14} class="text-blue-500" />
									<span class="font-medium text-sm text-gray-900">425 Market Street</span>
								</div>
								<p class="text-xs text-gray-500">Office • 15,000 SF • Downtown</p>
							</div>
							<div class="text-right">
								<div class="text-sm font-semibold text-gray-900">$4.2M</div>
								<span class="px-2 py-0.5 bg-green-100 text-green-700 text-[10px] rounded-full">Negotiation</span>
							</div>
						</div>

						<!-- Deal 2 -->
						<div class="flex items-center justify-between p-3 bg-gray-50 rounded-lg">
							<div class="flex-1">
								<div class="flex items-center gap-2 mb-1">
									<Building2 size={14} class="text-purple-500" />
									<span class="font-medium text-sm text-gray-900">Riverside Retail Plaza</span>
								</div>
								<p class="text-xs text-gray-500">Retail • 8,500 SF • Midtown</p>
							</div>
							<div class="text-right">
								<div class="text-sm font-semibold text-gray-900">$2.8M</div>
								<span class="px-2 py-0.5 bg-blue-100 text-blue-700 text-[10px] rounded-full">Qualified</span>
							</div>
						</div>

						<!-- Deal 3 -->
						<div class="flex items-center justify-between p-3 bg-gray-50 rounded-lg">
							<div class="flex-1">
								<div class="flex items-center gap-2 mb-1">
									<Building2 size={14} class="text-orange-500" />
									<span class="font-medium text-sm text-gray-900">Warehouse District 7</span>
								</div>
								<p class="text-xs text-gray-500">Industrial • 45,000 SF • Eastside</p>
							</div>
							<div class="text-right">
								<div class="text-sm font-semibold text-gray-900">$8.5M</div>
								<span class="px-2 py-0.5 bg-yellow-100 text-yellow-700 text-[10px] rounded-full">Prospecting</span>
							</div>
						</div>
					</div>
				</div>
				
				<!-- Decorative geometric shape -->
				<div class="absolute bottom-10 right-10 opacity-20">
					<svg width="100" height="100" viewBox="0 0 100 100" fill="none">
						<circle cx="50" cy="50" r="40" stroke="black" stroke-width="1"/>
						<path d="M50 10 C 70 30, 70 70, 50 90 C 30 70, 30 30, 50 10" stroke="black" stroke-width="1" fill="none"/>
						<path d="M10 50 C 30 30, 70 30, 90 50 C 70 70, 30 70, 10 50" stroke="black" stroke-width="1" fill="none"/>
					</svg>
				</div>
			</div>
		</div>

		<!-- Row 3: Property tracking -->
		<div class="grid grid-cols-1 md:grid-cols-3">
			<div class="p-12 flex flex-col justify-between border-r border-gray-200">
				<div>
					<h3 class="text-xl font-bold text-gray-900 mb-4">Property tracking</h3>
					<p class="text-gray-500 leading-relaxed mb-8">
						Centralize property data, market comps, and listing details. Everything you need to move deals forward in one place.
					</p>
				</div>
			</div>
			<div class="col-span-2 bg-gray-50/50 p-12 flex items-center justify-center relative">
				<div class="bg-white rounded-xl shadow-sm border border-gray-200 w-full max-w-lg overflow-hidden">
					<div class="p-4 border-b border-gray-100 flex items-center justify-between">
						<div class="flex items-center gap-2">
							<Building2 size={16} class="text-blue-500" />
							<h4 class="font-semibold text-gray-900">425 Market Street</h4>
						</div>
						<span class="px-2 py-1 bg-blue-50 text-blue-700 text-xs rounded">Office</span>
					</div>
					<div class="p-4 space-y-4">
						<div class="grid grid-cols-2 gap-4 text-sm">
							<div>
								<div class="text-xs text-gray-500 mb-1">Size</div>
								<div class="font-medium text-gray-900">15,000 SF</div>
							</div>
							<div>
								<div class="text-xs text-gray-500 mb-1">Price</div>
								<div class="font-medium text-gray-900">$4.2M</div>
							</div>
							<div>
								<div class="text-xs text-gray-500 mb-1">Location</div>
								<div class="font-medium text-gray-900">Downtown</div>
							</div>
							<div>
								<div class="text-xs text-gray-500 mb-1">Status</div>
								<div class="font-medium text-gray-900">Available</div>
							</div>
						</div>
						<div class="border-t border-gray-100 pt-4">
							<div class="text-xs text-gray-500 mb-2">Recent Activity</div>
							<div class="space-y-2 text-xs">
								<div class="flex items-center gap-2 text-gray-600">
									<div class="w-1.5 h-1.5 rounded-full bg-green-500"></div>
									<span>Tour scheduled for tomorrow</span>
								</div>
								<div class="flex items-center gap-2 text-gray-600">
									<div class="w-1.5 h-1.5 rounded-full bg-blue-500"></div>
									<span>Proposal sent to client</span>
								</div>
								<div class="flex items-center gap-2 text-gray-600">
									<div class="w-1.5 h-1.5 rounded-full bg-gray-400"></div>
									<span>Market comp analysis completed</span>
								</div>
							</div>
						</div>
					</div>
				</div>
				
				<!-- Decorative geometric shape -->
				<div class="absolute bottom-10 right-10 opacity-20">
					<svg width="100" height="100" viewBox="0 0 100 100" fill="none">
						<rect x="25" y="25" width="50" height="50" stroke="black" stroke-width="1" transform="rotate(45 50 50)"/>
						<rect x="25" y="25" width="50" height="50" stroke="black" stroke-width="1"/>
					</svg>
				</div>
			</div>
		</div>
	</div>
</section>
