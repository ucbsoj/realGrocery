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

    <h2>The Deals</h2>  

    <div class="grid">
        {#each [1] as i}
           <Image src="assets/images/meatbanner.png" alt="A lake and some clouds"/>
        {/each}

        {#each [2] as i}
        <Image src="assets/images/dairybanner.png" alt="A lake and some clouds"/>

        {/each}

        {#each [3] as i}
        <Image src="assets/images/groceryoutlet.JPG" alt="A lake and some clouds" caption="Lakeshore Trader Joes, <strong> Oakland </strong> "/>     {/each}

     {#each [4] as i}
        <Image src="assets/images/foodmaxx.jpeg" alt="A lake and some clouds" caption="University Trader Joes, <strong> Berkeley </strong> "/>
     {/each}
   
   
    </div>

    <div class="blocker">

    </div>

    <div class="grid">
        {#each [1] as i}
           <Image src="assets/images/wheatbanner.png" alt="A lake and some clouds" />
        {/each}

        {#each [2] as i}
        <Image src="assets/images/fruitbanner.png" alt="A lake and some clouds"/>

        {/each}

        {#each [3] as i}
        <Image src="assets/images/traderoak.jpg" alt="A lake and some clouds" caption="Lakeshore Trader Joes (Again), <strong> Oakland </strong>"/>
     {/each}

     {#each [4] as i}
     <Image src="assets/images/groceryoutlet.JPG" alt="A lake and some clouds" caption="Broadway Grocery Outlet, <strong> Oakland </strong>"
/>
     {/each}
   
   
    </div>

   <!-- For Passer if wanted 
    
   <div class="passer">
        <p>So how'd we get here?</p>
    </div>
-->
 
    
  
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
        padding: -30px;
        padding-bottom: 50px;
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
        padding-top: 20px;
    }

    .blocker{
        display: block;
        padding-top: 40px;
        padding-bottom: 5px;
    }

    h2{
		font-family: "Faster One";
	}

	p{
		font-family: "Quantico";
	}

</style>

