<script>
	import Header from '../components/Header.svelte';
</script>

<Header/>

<div class="container px-4">
	<h1 class="text-4xl font-bold mb-8">Order</h1>

	<dl>
		<dt>Espresso</dt>
		<dd>
			2,800
			<button class="btn btn-sm btn-outline-secondary">Select</button>
		</dd>
		<dt>Americano</dt>
		<dd>
			3,000
			<button class="btn btn-sm btn-outline-secondary">Select</button>
		</dd>
	</dl>

	<hr class="my-4">

	<h2 class="text-2xl font-bold mb-2">Order Sheet</h2>

	Total: 0
</div>