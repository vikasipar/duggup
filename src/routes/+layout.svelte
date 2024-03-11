<script>
	import "../app.css";
	import Intro from "../components/Intro.svelte";
	import Header from '../components/Header.svelte';
	import './styles.css';
	let intro = true;
	setTimeout(()=>intro=false, 2000);
</script>

{#if intro}
<Intro/>
{:else}
<div>
	<Header />
	<main>
		<slot />
	</main>
</div>
{/if}