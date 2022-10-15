<script>
	import { Router, Route } from 'svelte-routing';
	import Home from './pages/Home.svelte';
	import About from './pages/About.svelte';
	import Order from './pages/Order.svelte';
</script>

<Router>
	<Route path="/" component={ Home } />
	<Route path="/about" component={ About } />
	<Route path="/order" component={ Order } />
</Router>

<style>
	
</style>