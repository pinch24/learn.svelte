<script>
	import Layout from '../components/Layout.svelte';
	import { navigate } from 'svelte-routing';
</script>

<Layout hideHeader={ true }>
	<section>
		<button 
			class="btn btn-outline-primary" 
			on:click={ () => navigate('/', { replace: true }) }
		>
			Login
		</button>
	</section>
</Layout>

<style>
	section {
		height: 50vh;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>