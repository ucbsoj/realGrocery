<script>
	import Image from "$components/helpers/Image.svelte";

	/*
		The Image component creates an image with an optional caption.
		- src: The source of the image file.
		- alt: The alt text for the image.
		- caption: The caption for the image.
		
		The image will take on the width and height of its container. To make the image smaller or larger,
		wrap it in a container of the size you want.
	*/
</script>

<section>

    <h2>A quick look at our cheapest stores by product</h2>  

    <div class="grid">
        {#each [1] as i}
           <Image src="assets/images/traderoak.jpg" alt="A lake and some clouds" caption="Lakeshore Trader Joes, <strong> Oakland </strong> <p> Lorem ipsum dolor, sit amet consectetur adipisicing elit. Hic, odit cum praesentium consequuntur quaerat quisquam facilis ex, reiciendis quasi quibusdam provident sed assumenda molestias, tenetur exercitationem aut odio at temporibus?</p>"/>
        {/each}

        {#each [2] as i}
        <Image src="assets/images/groceryoutlet.JPG" alt="A lake and some clouds" caption="Broadway Grocery Outlet, <strong> Oakland </strong>     <p> Lorem ipsum dolor, sit amet consectetur adipisicing elit. Hic, odit cum praesentium consequuntur quaerat quisquam facilis ex, reiciendis quasi quibusdam provident sed assumenda molestias, tenetur exercitationem aut odio at temporibus?</p>
"/>
        {/each}

        {#each [3] as i}
        <Image src="assets/images/traderoak.jpg" alt="A lake and some clouds" caption="Lakeshore Trader Joes, <strong> Oakland </strong> <p> Lorem ipsum dolor, sit amet consectetur adipisicing elit. Hic, odit cum praesentium consequuntur quaerat quisquam facilis ex, reiciendis quasi quibusdam provident sed assumenda molestias, tenetur exercitationem aut odio at temporibus?</p>"/>
     {/each}

     {#each [4] as i}
     <Image src="assets/images/groceryoutlet.JPG" alt="A lake and some clouds" caption="Broadway Grocery Outlet, <strong> Oakland </strong>     <p> Lorem ipsum dolor, sit amet consectetur adipisicing elit. Hic, odit cum praesentium consequuntur quaerat quisquam facilis ex, reiciendis quasi quibusdam provident sed assumenda molestias, tenetur exercitationem aut odio at temporibus?</p>
"/>
     {/each}
   
   
    </div>
    <div class="passer">
        <p>So how'd we get here?</p>
    </div>
    
  
</section>

<style>
   
	.small {
		width: 300px;
		margin: 36px auto;
	}

	.grid {
		display: grid;
        grid-template-columns: repeat(2, 1fr);
		gap: 16px;
        row-gap: 200px;
        padding-bottom: 30px;
	}


	section {
		background: #FFEAEA;
		max-width: 600px;
		margin: 20px auto;
		padding: 10px;
		border-radius: 10px;
        
	}

    h2, p{
        text-align: center;
    }

    .passer{
        display: block;
        padding-top: 200px;
    }

</style>