<script>
	let diameter = 1;
	let height = 1;

	$: volume = area * height;
	$: area = Math.PI * radius ** 2;
	$: radius = diameter / 2;
</script>

<main>
	<h1>Cylinder Calculations</h1>
	<label>
		Diameter <input type="number" bind:value={ diameter }>
	</label>
	<label>
		Height <input type="number" bind:value={ height }>
	</label>
	<label>Radius: { radius }</label>
	<label>Area: { area.toFixed(2) }</label>
	<label>Volume: { volume.toFixed(2) }</label>
</main>

<style>
	input {
		width: 50px;
	}
</style>