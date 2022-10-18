<script>
    import { element } from 'svelte/internal';
    import About from '../pages/About.svelte';
	import Header from '../components/Header.svelte';

	const formatter = Intl.NumberFormat('ko-KR');

	const menu = [
		{ name: 'Esprosso', price: 2800 },
		{ name: 'Americano', price: 3000 },
		{ name: 'Cafe Latte', price: 3400 },
		{ name: 'Vanilla Latte', price: 3700 },
	]

	let selected = [];

	function toggleItem(name) {
		if (selected.find(element => element.name === name)) {
			selected = selected.filter(element => element.name !== name);
		}
		else {
			const item = menu.find(element => element.name === name);
			selected = [...selected, item];
		}
	}

	let sum = 0;
	$: {
		sum = 0;
		selected.forEach(item => sum += item.price);
	}
</script>

<Header/>

<div class="container px-4">
	<h1 class="text-4xl font-bold mb-8">Order</h1>

	<dl>
		{ #each menu as item }
			<dt>{ item.name }</dt>
			<dd>
				{ formatter.format(item.price) }
				<button class="btn btn-sm btn-outline-primary" on:click={ () => toggleItem(item.name) }>
					{ selected.find(element => element.name === item.name) ? 'Selected' : 'Select' }
				</button>
			</dd>
		{ /each }
	</dl>

	<hr class="my-4">

	<h2 class="text-2xl font-bold mb-2">Order Sheet</h2>

	<ul class="mb-2">
		{ #each selected as item }
			<li>- { item.name} </li>
		{ /each }
	</ul>

	<p>Sum: {formatter.format(sum)}</p>
</div>