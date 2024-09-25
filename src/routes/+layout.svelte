<script>
  import '../app.css'
	import Navbar from '$lib/Navbar/Navbar.svelte';
	import Footer from '$lib/Footer/Footer.svelte';
</script>

<Navbar />

<div class="container">
	<slot></slot>
</div>

<Footer />

<style>
	.container {
		display: flex;
		justify-content: stretch;
		flex-direction: column;
	}
</style>
