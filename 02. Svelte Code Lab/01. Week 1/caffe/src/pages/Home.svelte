<script>
	import Header from '../components/Header.svelte';
	import { navigate } from 'svelte-routing';

	function goOrder() {
		// do gtag
		navigate('/order');
	}
</script>

<Header/>

<div class="container px-4">
	<h1 class="text-4xl font-bold my-8">Caffe</h1>
	<p class="mb-4">Online Coffee Order Service</p>
	<button class="btn btn-outline-primary" on:click={ goOrder }>Now Order</button>
</div>