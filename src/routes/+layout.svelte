<script>
	import Footer from '$lib/components/Footer.svelte';
import Navbar from '$lib/components/Navbar.svelte';
	import '../app.css';
</script>

<div class="px-24">
	<Navbar />
	<slot />
	<Footer />
</div>
