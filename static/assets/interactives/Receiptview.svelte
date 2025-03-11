<script>
	import Receipt from '$assets/interactives/Receipt.svelte';
</script>

<div class="horizontal-wrapper">
	<Receipt/>
	<Receipt/>
	<Receipt/>
</div>

<style>
	.horizontal-wrapper {
		display: flex;
		flex-direction: row;
		gap: 10px;
	}
</style>