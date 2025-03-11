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

    <h2>So how did everyone do product by product? </h2>  

    <div class="grid">
        {#each [1] as i}
           <Image src="assets/images/dairy.png" alt="diary icon" caption="Dairy"/>
        {/each}

        {#each [2] as i}
        <Image src="assets/images/1meat.png" alt="meat icon" caption="Meat"/>

        {/each}

        {#each [3] as i}
       
		<div class="foodItems">
			<ol>
		
				<li>Trader Joes Berkeley</li>
				<li>Grocery Outlet Oakland</li>
				<li>Trader Joes Oakland</li>
				<li>Foodmaxx Oakland</li>
				<li>Whole Foods Oakland</li>
				<li>Berkeley Bowl Berkeley</li>

			</ol>

		</div>
     {/each}

	 {#each [4] as i}
       
	 <div class="foodItems">
		 <ol>
	 
			 <li>Grocery Outlet Oakland</li>
			 <li>Foodmaxx Oakland</li>
			 <li>Trader Joes Oakland</li>
			 <li>Trader Joes Berkeley</li>
			 <li>Whole Foods Oakland</li>
			 <li>Berkeley Bowl Berkeley</li>

		 </ol>

	 	</div>
	  {/each}	
	 </div>
 
	
	 <div class="grid">
        {#each [1] as i}
           <Image src="assets/images/onion.png" alt="veggie icon" caption="<strong>Fruits/Veggies</strong>"/>
        {/each}

        {#each [2] as i}
        <Image src="assets/images/bread.png" alt="bread icon" caption="Wheat/Grains"/>

        {/each}

        {#each [3] as i}
       
		<div class="foodItems">
			<ol>
				<li>Grocery Outlet Oakland</li>
				<li>Foodmaxx Oakland</li>
				<li>Berkeley Bowl Berkeley</li>
				<li>Trader Joes Oakland</li>
				<li>Trader Joes Berkeley</li>
				<li>Whole Foods Oakland</li>
				

			</ol>

		</div>
     {/each}

	 {#each [4] as i}
       
	 <div class="foodItems">
		 <ol>
	 
			 <li>Trader Joes Oakland</li>
			 <li>Trader Joes Berkeley</li>
			 <li>Foodmaxx Oakland</li>
			 <li>Grocery Outlet Oakland</li>
			 <li>Whole Foods Oakland</li>
			 <li>Berkeley Bowl Berkeley</li>

		 </ol>

	 </div>
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
		gap: 10px;
        row-gap: 30px;
        padding-bottom: 10px;
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

	.foodItems{
		display: block;
		padding-left: 40px;
		background-image: src="test.notepad.png";
	}

</style>