<script>
	import { Link, link } from 'svelte-routing';
</script>

<header class="container flex justify-between">
	<a href="/" class="btn btn-link text-black text-2xl font-bold no-underline" use:link>Caffe</a>
	<nav>
		<Link class="btn btn-link" to="/">Home</Link>
		<Link class="btn btn-link" to="about">About</Link>
		<Link class="btn btn-link" to="order">Order</Link>
		<Link class="btn btn-link" to="signin">Login</Link>
	</nav>
</header>