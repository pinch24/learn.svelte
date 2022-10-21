<script>
	let status = 200;
	let message = "This is a message.";

	$: error = status >= 200;
</script>

<main>
	<label>
		Status <input type="number" bind:value={ status }>
	</label>

	<div class:error>{ message }</div>
</main>

<style>
	.error {
		color: red;
		font-weight: bold;
	}
</style>