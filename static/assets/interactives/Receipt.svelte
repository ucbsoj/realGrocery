<script>
	let stores = [
		"99 Ranch",
		"Berkeley Bowl",
		"Cardenas",
		"Foodmaxx"
	]

	let longStores = new Array(100).fill("99 Ranch");
</script>

<div class="receipt">
	<div class="name">Bread</div>
	<div class="description">Loaf of white bread</div>

	<ul>
		{#each longStores as s}
			<li>{s}</li>
		{/each}
	</ul>
</div>

<style>
	.receipt {
		background: lightgray;
		width: 200px;
		max-height: 400px;
		overflow: scroll;
	}

	.name {
		font-weight: bold;
		text-align: center;
	}

	.description {
		font-size: 14px;
		text-align: center;
	}
</style>