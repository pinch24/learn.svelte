<script>
	let value = Math.random();
	function showAnotherUniverse() {
		value = Math.random();
	}
</script>

<main>
	<p>
		{ value } is  { value < 0.5 ? 0 : 1 }
	</p>
	<button on:click={ showAnotherUniverse }>Reset</button>
</main>

<style>
	main {
		width: 100vw;
		height: 100vh;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	p {
		font-size: 2rem;
		font-weight: bold;
	}
</style>