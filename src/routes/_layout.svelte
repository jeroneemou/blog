<script>
import AppBar from '../components/AppBar.svelte';
</script>

<style global lang="scss">
	@import '../styles/global.scss';	
</style>


<svelte:head>

</svelte:head>

<AppBar/>
<main>
	<slot />
</main>