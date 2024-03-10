<script>
	import "../app.css";
	import Header from './Header.svelte';
	// import './styles.css';
</script>

<div class="w-[100vw] mx-0 px-0">
	<Header />
	<main>
		<slot />
	</main>
</div>