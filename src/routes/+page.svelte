<script lang="ts">
	import Navbar from '$lib/Navbar.svelte';
	import Hero from '$lib/Hero.svelte';
	import Features from '$lib/Features.svelte';
	import CTA from '$lib/CTA.svelte';
	import Footer from '$lib/Footer.svelte';
</script>

<Navbar />
<main class="bg-white min-h-screen">
	<Hero />
	<Features />
	<CTA />
</main>
<Footer />

