<script>
import Receipt from "$components/interactives/Receipt.svelte"

let selectedStore = $state("Whole Foods")
$inspect(selectedStore)

</script>

<section>
	<h2>Check out products by store here!</h2>

	<p>We wanted to explore what grocery prices were like, right here in our own East Bay backyard. Right now, everything feels more expensive, and we hope that this project can provide locals with a snapshot of what their prices are doing. </p>
    
    <p>In the U.S. Grocery increased 2.1% in the year of 2024. Egg prices are in the news everyday. Consumer are voicing their fears amidst looming agricultural tariffs. Everywhere people are talking about prices.</p>
    <p>So how are your prices doing?</p>

	<select bind:value={selectedStore}>
		<option>Whole Foods</option>
		<option>Trader Joes Berkeley</option>
		<option>Foodmaxx</option>
		<option>Trader Joes Oakland</option>
		<option>Grocery Outlet</option>
		<option>Berkeley Bowl</option>
	</select>


    <div class="horizontal-wrapper">
        <Receipt name={"Dairy"} description={"List of Dairy Products"} items={["a","b","c"]}/>
		<Receipt name={"Dairy"} description={"List of Dairy Products"} items={["a","b","c"]}/>
		<Receipt name={"Dairy"} description={"List of Dairy Products"} items={["a","b","c"]}/>
		<Receipt name={"Dairy"} description={"List of Dairy Products"} items={["a","b","c"]}/>

		
    </div>
  

</section>

<style>


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



	.horizontal-wrapper {
		display: flex;
		flex-direction: row;
		gap: 10px;
		overflow-x: scroll;
		overflow: hidden;
	}


</style>