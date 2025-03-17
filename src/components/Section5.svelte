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

    <h2>The Product Rankings </h2> 
	

    <div class="grid">
        {#each [1] as i}
           <Image src="assets/images/dairy.png" alt="diary icon" caption="<strong>Dairy</strong>"/>
        {/each}

        {#each [2] as i}
        <Image src="assets/images/1meat.png" alt="meat icon" caption="<strong>Meat</strong>"/>

        {/each}

        {#each [3] as i}
       
		<div class="foodItems">
			<ol>
		
				<li>Trader Joes Berkeley: <strong>$22.35</strong></li>
				<li>Grocery Outlet: <strong>$22.75</strong></li>
				<li>Trader Joes Oakland: <strong>$22.85</strong></li>
				<li>Foodmaxx: <strong>$23.25</strong></li>
				<li>Whole Foods: <strong>$24.95</strong></li>
				<li>Berkeley Bowl: <strong>$26.75</strong></li>

			</ol>

		</div>
     {/each}

	 {#each [4] as i}
       
	 <div class="foodItems">
		 <ol>
	 
			 <li>Grocery Outlet: <strong>$22.15</strong> </li>
			 <li>Foodmaxx: <strong>$25.75</strong> </li>
			 <li>Trader Joes Oakland: <strong>$30.95</strong></li>
			 <li>Trader Joes Berkeley: <strong>$30.95</strong></li>
			 <li>Whole Foods: <strong>$32.95</strong> </li>
			 <li>Berkeley Bowl: <strong>$37.45</strong></li>

		 </ol>

	 	</div>
	  {/each}	
	 </div>
 
	
	 <div class="grid">
        {#each [1] as i}
           <Image src="assets/images/onion.png" alt="veggie icon" caption="<strong>Fruits/Veggies</strong>"/>
        {/each}

        {#each [2] as i}
        <Image src="assets/images/bread.png" alt="bread icon" caption="<strong>Wheat/Grains</strong>"/>

        {/each}

        {#each [3] as i}
       
		<div class="foodItems">
			<ol>
				<li>Grocery Outlet: <strong>$9.33</strong> </li>
				<li>Foodmaxx: <strong>$9.38</strong></li>
				<li>Berkeley Bowl: <strong>$10.13</strong></li>
				<li>Trader Joes Oakland: <strong>$10.51</strong></li>
				<li>Trader Joes Berkeley: <strong>$11.90</strong></li>
				<li>Whole Foods: <strong>$16.33</strong> </li>
				

			</ol>

		</div>
     {/each}

	 {#each [4] as i}
       
	 <div class="foodItems">
		 <ol>
	 
			 <li>Trader Joes Oakland: <strong>$6.56</strong></li>
			 <li>Trader Joes Berkeley: <strong>$8.06</strong></li>
			 <li>Foodmaxx: <strong>$9.22</strong> </li>
			 <li>Grocery Outlet: <strong>$9.41</strong> </li>
			 <li>Whole Foods: <strong>$11.36</strong> </li>
			 <li>Berkeley Bowl: <strong>$15.56</strong> </li>

		 </ol>

	 </div>
     {/each}
    </div>
	
   <!-- <div class="passer">
        <p>So how'd we get here?</p>
    </div>

	-->
    
  
	<p>Each store was ranked by comparing the total price of a popular food product basket in all four major food categories we analyzed:</p>
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
		padding-left: 30px;
		background-image: url("$assets/images/paper.png");
		font-family: "Quantico";
	}

</style>