<script>
	import "../app.css";
	import Header from './Header.svelte';
	import './styles.css';
</script>

<div>
	<Header />
	<main class="">
		<slot />
	</main>
</div>