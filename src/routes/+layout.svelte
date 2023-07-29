<script>
	import Footer from '$lib/components/Footer.svelte';
	import Navbar from '$lib/components/Navbar.svelte';
	import '../app.css';
</script>

<svelte:head>
	<!-- Primary Tags -->
	<title>E-SEVEN • Muziek Voor Bruiloften En Andere Evenementen</title>
	<meta name="title" content="E-SEVEN • Muziek Voor Bruiloften En Andere Evenementen" />
	<meta
		name="description"
		content="Wij zijn drie vrienden die al jaren muziek maken. Wij spelen graag op bruiloften of andere evenementen met ons gevarieerde repetoire."
	/>
	<meta
		name="keywords"
		content="muziek,band,evenement,evenementen,bruiloft,fullband,akoestisch,hester,jonathan,janicke"
	/>
	<meta name="language" content="NL" />
	<meta name="author" content="Fyxren" />

	<!-- Open Graph -->
	<meta property="og:type" content="website" />
	<meta property="og:url" content="https://metatags.io" />
	<meta property="og:title" content="E-SEVEN • Muziek Voor Bruiloften En Andere Evenementen" />
	<meta
		property="og:description"
		content="Wij zijn drie vrienden die al jaren muziek maken. Wij spelen graag op bruiloften of andere evenementen met ons gevarieerde repetoire."
	/>
	<meta property="og:image" content="https://i.postimg.cc/4y5g2mfD/e-seven-logo.jpg" />

	<!-- Twitter -->
	<meta property="twitter:card" content="summary_large_image" />
	<meta property="twitter:url" content="https://metatags.io" />
	<meta property="twitter:title" content="E-SEVEN • Muziek Voor Bruiloften En Andere Evenementen" />
	<meta
		property="twitter:description"
		content="Wij zijn drie vrienden die al jaren muziek maken. Wij spelen graag op bruiloften of andere evenementen met ons gevarieerde repetoire."
	/>
	<meta property="twitter:image" content="https://i.postimg.cc/4y5g2mfD/e-seven-logo.jpg" />
</svelte:head>

<div class="px-5 md:px-24">
	<Navbar />
	<slot />
	<Footer />
</div>
