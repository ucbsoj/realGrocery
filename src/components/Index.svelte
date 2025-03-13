<script>
	import Demo from "$components/demo/Demo.svelte";
	import Footer from "$components/Footer.svelte";
	import Hero from "$components/helpers/Hero.svelte";
	import Section1 from '$components/Section1.svelte';
	import Section2 from '$components/Section2.svelte';
	import Section3 from '$components/Section3.svelte';
	import Section4 from '$components/Section4.svelte';
	import Section5 from '$components/Section5.svelte';
	import Section6 from "$components/Section6.svelte";
	import Section7 from "$components/Section7.svelte";
//	import Section8 from "$components/Section8.svelte";
</script>

<Hero
	hed="Grocery Madness"
	dek="A guide for savvy shopping in the East Bay"
	byline="From Edith Matthias, Marquis Chambers, and Xavey Bzdek"
	src="assets/images/GMheader.JPG"
	alt="A lake and some clouds"
/>

<Section1/>

<Section2/>

<Section3/>

<Section4/>

<Section5/>

<Section6/>

<Section7/>



<Footer />

<style>
	:global(body) {
		background: #58BA8C;
	}
	
	:global(h2) {
		font-family: "Faster One";
		background-color: #58BA8C;
		border-radius: 5px;
		padding: 10px;
	}

	:global(p) {
		font-family: "Quantico";
	}

	
</style>