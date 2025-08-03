<script>
	import '../app.css';
	import Navbar from '$lib/components/Navbar.svelte';
	import Footer from '$lib/components/Footer.svelte';
</script>

<svelte:head>
	<title>Burbsec | The World's Most Fun InfoSec Meetup Events!</title>
	<meta name="description" content="The World's Most Fun Information Security Meetup Network" />
</svelte:head>

<Navbar />
<main>
	<slot />
</main>
<Footer />

<style>
	:global(body) {
		background-color: #15202b;
		min-height: 100vh;
		color: white;
	}
	
	main {
		min-height: calc(100vh - 200px);
	}
</style>