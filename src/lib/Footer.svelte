<script lang="ts">
	import { Twitter, Linkedin, Github, Youtube } from 'lucide-svelte';
</script>

<footer class="bg-black text-white pt-20 pb-10 px-6">
	<div class="max-w-[1200px] mx-auto">
		<div class="flex flex-col md:flex-row items-start justify-between gap-12 mb-12">
			<!-- Logo Column -->
			<div class="max-w-sm">
				<a href="/" class="flex items-center gap-2 text-white mb-6">
					<svg width="24" height="26" viewBox="0 0 97 105" fill="none" xmlns="http://www.w3.org/2000/svg">
						<path opacity="0.5" d="M0.84375 29.5892V75.3785L43.791 45.7896V0L0.84375 29.5892Z" fill="white"/>
						<path opacity="0.5" d="M0.84375 75.3787V29.5891L43.791 59.1783V104.968L0.84375 75.3787Z" fill="white"/>
						<path opacity="0.5" d="M96.8438 29.5891V75.3787L53.8965 45.7895V0L96.8438 29.5891Z" fill="white"/>
						<path opacity="0.5" d="M96.8438 75.3787V29.5891L53.8965 59.1783V104.968L96.8438 75.3787Z" fill="white"/>
					</svg>
					<span class="font-bold text-xl tracking-tight">Renlo</span>
				</a>
				<p class="text-sm text-gray-400 leading-relaxed">
					The AI-native CRM built for commercial real estate brokers. Close more deals, faster.
				</p>
			</div>

			<!-- Contact -->
			<div>
				<h4 class="text-sm font-medium text-gray-400 mb-4">Get in touch</h4>
				<a href="#" class="inline-block bg-white text-black text-sm font-medium px-5 py-2.5 rounded-lg hover:bg-gray-200 transition-colors">
					Book a call
				</a>
			</div>
		</div>

		<div class="border-t border-gray-800 pt-8 flex flex-col md:flex-row items-center justify-between gap-4">
			<div class="flex items-center gap-6">
				<a href="#" class="text-gray-500 hover:text-white transition-colors"><Linkedin size={20} /></a>
			</div>
			
			<div class="flex items-center gap-6 text-xs text-gray-500">
				<span>© 2025 Renlo. All rights reserved.</span>
				<a href="#" class="hover:text-gray-300">Privacy Policy</a>
			</div>
		</div>
	</div>
</footer>
