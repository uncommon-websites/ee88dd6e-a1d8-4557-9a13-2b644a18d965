<script lang="ts">
	import { ArrowRight, ChevronDown, Search, Bell, CheckSquare, Mail, BarChart2, Zap, Layout, Users, Briefcase, Building2, Plus, MoreHorizontal, Filter, RefreshCw, Download } from 'lucide-svelte';
</script>

<section class="pt-24 pb-20 px-6 text-center max-w-[1400px] mx-auto">
	<div class="inline-flex items-center gap-2 text-xs font-medium text-gray-500 mb-8 border border-gray-200 rounded-full px-3 py-1 bg-white">
		<span class="w-2 h-2 bg-green-500 rounded-full animate-pulse"></span>
		Early Access
	</div>

	<h1 class="text-[56px] leading-[1.1] font-serif tracking-tight text-gray-900 mb-6 max-w-4xl mx-auto">
		The Modern OS for High-Performance Brokers
	</h1>

	<p class="text-lg text-gray-500 mb-10 max-w-xl mx-auto text-balance">
		Unify relationships, deals, properties, and activity into a single system. Move faster, stay organized, close more transactions.
	</p>

	<div class="flex items-center justify-center gap-4 mb-20">
		<a href="#" class="bg-black text-white text-sm font-medium px-5 py-2.5 rounded-lg hover:bg-gray-800 transition-colors">
			Book a call
		</a>
	</div>

	<!-- Dashboard Preview -->
	<div class="relative rounded-xl overflow-hidden shadow-2xl border border-gray-200 bg-white text-left mx-auto max-w-[1200px]">
		<!-- Tabs -->
		<div class="flex border-b border-gray-200 bg-gray-50/50">
			<button class="px-8 py-3 text-xs font-medium text-gray-500 hover:text-black border-b-2 border-transparent">Properties</button>
			<button class="px-8 py-3 text-xs font-medium text-black border-b-2 border-black bg-white">Deals</button>
			<button class="px-8 py-3 text-xs font-medium text-gray-500 hover:text-black border-b-2 border-transparent">Relationships</button>
			<button class="px-8 py-3 text-xs font-medium text-gray-500 hover:text-black border-b-2 border-transparent">Activity</button>
		</div>

		<!-- UI Container -->
		<div class="flex h-[600px] bg-white">
			<!-- Sidebar -->
			<div class="w-[240px] border-r border-gray-200 flex flex-col text-[13px] text-gray-600">
				<div class="p-3 flex items-center gap-2 font-medium text-black border-b border-gray-100">
					<div class="w-5 h-5 bg-black rounded flex items-center justify-center text-white text-[10px]">R</div>
					Renlo
					<ChevronDown size={14} class="ml-auto opacity-50" />
				</div>
				
				<div class="p-2 space-y-0.5">
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Search size={14} /> Quick actions
						<div class="ml-auto text-[10px] border border-gray-200 rounded px-1">⌘K</div>
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Bell size={14} /> Notifications
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<CheckSquare size={14} /> Tasks
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 bg-gray-100 text-black font-medium rounded cursor-pointer">
						<Briefcase size={14} /> Deals
					</div>
				</div>

				<div class="mt-2 px-4 text-[11px] font-medium text-gray-400">Records</div>
				<div class="p-2 space-y-0.5">
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Building2 size={14} class="text-blue-500" /> Properties
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Users size={14} class="text-green-500" /> Relationships
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Briefcase size={14} class="text-orange-500" /> Deals
					</div>
					<div class="flex items-center gap-2 px-2 py-1.5 hover:bg-gray-50 rounded cursor-pointer">
						<Layout size={14} class="text-purple-500" /> Activity
					</div>
				</div>
			</div>

			<!-- Main Content -->
			<div class="flex-1 flex flex-col bg-gray-50/30">
				<!-- Header -->
				<div class="h-14 border-b border-gray-200 flex items-center justify-between px-6 bg-white">
					<div class="flex items-center gap-2 text-sm text-gray-500">
						<Briefcase size={16} />
						<span>Deals</span>
						<span class="text-gray-300">/</span>
						<span class="text-black font-medium">Active Pipeline</span>
					</div>
					<div class="flex items-center gap-3">
						<div class="flex -space-x-2">
							<div class="w-6 h-6 rounded-full bg-blue-100 border-2 border-white flex items-center justify-center text-[10px]">JM</div>
							<div class="w-6 h-6 rounded-full bg-green-100 border-2 border-white flex items-center justify-center text-[10px]">SK</div>
						</div>
						<button class="text-xs font-medium text-gray-600 hover:text-black flex items-center gap-1">
							Share
						</button>
					</div>
				</div>

				<!-- Dashboard Content -->
				<div class="p-6 overflow-hidden">
					<div class="mb-6 flex items-center justify-between">
						<div>
							<h2 class="text-lg font-semibold text-gray-900">Active Pipeline</h2>
							<p class="text-sm text-gray-500">Track your deals across stages, monitor property activity, and close faster.</p>
						</div>
						<div class="flex items-center gap-2">
							<button class="text-xs font-medium text-gray-500 hover:text-black flex items-center gap-1 px-2 py-1">
								<Filter size={12} /> Filter
							</button>
							<button class="bg-black text-white text-xs font-medium px-3 py-1.5 rounded-md hover:bg-gray-800 flex items-center gap-1">
								<Plus size={12} /> Add deal
							</button>
						</div>
					</div>

					<div class="grid grid-cols-5 gap-6 h-full">
						<!-- Chart 1: Deal flow -->
						<div class="col-span-3 bg-white rounded-lg border border-gray-200 p-4 shadow-sm">
							<div class="flex items-center justify-between mb-4">
								<h3 class="text-sm font-medium text-gray-900">Deal flow by property type</h3>
								<MoreHorizontal size={14} class="text-gray-400" />
							</div>
							<div class="flex items-center gap-4 text-[10px] text-gray-500 mb-4">
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-blue-400"></div> Office</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-green-400"></div> Retail</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-purple-400"></div> Industrial</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-orange-400"></div> Multifamily</div>
							</div>
							
							<!-- Mock Bar Chart -->
							<div class="relative h-[250px] w-full mt-8">
								<!-- Y Axis Labels -->
								<div class="absolute left-0 top-0 bottom-0 w-8 flex flex-col justify-between text-[10px] text-gray-400 text-right pr-2">
									<span>28</span>
									<span>24</span>
									<span>20</span>
									<span>16</span>
									<span>12</span>
									<span>8</span>
									<span>4</span>
								</div>
								<!-- Bars -->
								<div class="ml-10 h-full flex items-end justify-between px-4 border-l border-b border-gray-100">
									<!-- Q1 -->
									<div class="w-8 flex flex-col gap-0.5 items-center group relative">
										<div class="w-full bg-blue-200 h-12 rounded-t-sm"></div>
										<div class="w-full bg-green-200 h-16"></div>
										<div class="w-full bg-purple-200 h-8"></div>
										<div class="w-full bg-orange-200 h-10"></div>
										<div class="absolute -bottom-6 text-[10px] text-gray-500">Q1</div>
									</div>
									<!-- Q2 -->
									<div class="w-8 flex flex-col gap-0.5 items-center relative">
										<div class="w-full bg-blue-300 h-16 rounded-t-sm"></div>
										<div class="w-full bg-green-300 h-20"></div>
										<div class="w-full bg-purple-300 h-12"></div>
										<div class="w-full bg-orange-300 h-14"></div>
										<div class="absolute -bottom-6 text-[10px] text-gray-500">Q2</div>
										
										<!-- Tooltip Mock -->
										<div class="absolute bottom-full mb-2 left-1/2 -translate-x-1/2 bg-gray-900 text-white text-[10px] px-2 py-1 rounded whitespace-nowrap z-10">
											Deal velocity <span class="text-green-400 ml-1">+32%</span>
										</div>
										<div class="absolute bottom-full mb-1 left-1/2 -translate-x-1/2 w-0 h-0 border-l-[4px] border-l-transparent border-r-[4px] border-r-transparent border-t-[4px] border-t-gray-900"></div>
									</div>
									<!-- Q3 -->
									<div class="w-8 flex flex-col gap-0.5 items-center relative">
										<div class="w-full bg-blue-400 h-20 rounded-t-sm"></div>
										<div class="w-full bg-green-400 h-24"></div>
										<div class="w-full bg-purple-400 h-16"></div>
										<div class="w-full bg-orange-400 h-18"></div>
										<div class="absolute -bottom-6 text-[10px] text-gray-500">Q3</div>
									</div>
								</div>
							</div>
						</div>

						<!-- Chart 2: Donut -->
						<div class="col-span-2 bg-white rounded-lg border border-gray-200 p-4 shadow-sm">
							<div class="flex items-center justify-between mb-4">
								<h3 class="text-sm font-medium text-gray-900">Deals by stage</h3>
								<MoreHorizontal size={14} class="text-gray-400" />
							</div>
							<div class="flex flex-wrap gap-2 text-[10px] text-gray-500 mb-8">
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-blue-500"></div> Prospecting</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-green-500"></div> Qualified</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-purple-500"></div> Negotiation</div>
								<div class="flex items-center gap-1"><div class="w-2 h-2 rounded-full bg-orange-400"></div> Closing</div>
							</div>

							<!-- Mock Donut Chart -->
							<div class="relative w-48 h-48 mx-auto">
								<svg viewBox="0 0 100 100" class="w-full h-full transform -rotate-90">
									<circle cx="50" cy="50" r="40" fill="transparent" stroke="#e5e7eb" stroke-width="16" /> <!-- Base -->
									<circle cx="50" cy="50" r="40" fill="transparent" stroke="#3b82f6" stroke-width="16" stroke-dasharray="70 251" stroke-dashoffset="0" /> <!-- Blue segment -->
									<circle cx="50" cy="50" r="40" fill="transparent" stroke="#22c55e" stroke-width="16" stroke-dasharray="60 251" stroke-dashoffset="-70" /> <!-- Green segment -->
									<circle cx="50" cy="50" r="40" fill="transparent" stroke="#a855f7" stroke-width="16" stroke-dasharray="50 251" stroke-dashoffset="-130" /> <!-- Purple segment -->
									<circle cx="50" cy="50" r="40" fill="transparent" stroke="#fb923c" stroke-width="16" stroke-dasharray="40 251" stroke-dashoffset="-180" /> <!-- Orange segment -->
								</svg>
								<div class="absolute inset-0 flex items-center justify-center flex-col">
									<span class="text-2xl font-bold text-gray-900">47</span>
									<span class="text-xs text-gray-500">Active</span>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</section>
