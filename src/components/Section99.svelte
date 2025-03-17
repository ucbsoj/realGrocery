<script>
  import Image from './helpers/Image.svelte';
  import { writable, derived } from 'svelte/store';

  // Store price data
  const storeData = {
    store1: {
      meat: [
        { name: "Chicken Breast", price: 5.99 },
        { name: "Ground Beef", price: 6.99 },
		{ name: "Ground Turkey", price: 6.49 },
		{ name: "Pork Chop", price: 6.99 },
		{ name: "Chicken Thigh", price: 6.49}
      ],
      dairy: [
        { name: "Gallon Milk", price: 5.19 },
        { name: "Dozen Eggs", price: 4.99 },
		{ name: "Shredded Cheese(12oz)", price: 3.99 },
		{ name: "Butter (8oz)", price: 5.49 },
		{ name: "Block Cheese(8oz)", price: 5.29 }
      ],
      produce: [
		{ name: "Roma Tomato", price: 2.99 },
		{ name: "Apple", price: 1.99 },
        { name: "Banana", price: 0.89 },
		{ name: "Broccoli", price: 3.49 },
		{ name: "Bag Spinach(10oz)", price: 3.79 },
		{ name: "Yellow Onion", price: 1.69 },
		{ name: "Potato", price: 1.49 }

      ],
      wheat: [
        { name: "White Bread", price: 3.99 },
		{ name: "Wheat Bread", price: 3.99 },
		{ name: "Spaghetti", price: 1.39 },
        { name: "Rice", price: 1.99 }
      ]
    },
    store2: {
      meat: [
        { name: "Chicken Breast", price: 6.99 },
        { name: "Ground Beef", price: 4.99 },
		{ name: "Ground Turkey", price: 4.99 },
		{ name: "Pork Chop", price: 7.99 },
		{ name: "Chicken Thigh", price: 5.99}
      ],
      dairy: [
        { name: "Gallon Milk", price: 4.39 },
        { name: "Dozen Eggs", price: 4.99 },
		{ name: "Shredded Cheese(12oz)", price: 3.79 },
		{ name: "Butter (8oz)", price: 4.69 },
		{ name: "Block Cheese(8oz)", price: 4.49 }
      ],
      produce: [
		{ name: "Roma Tomato", price: 1.16 },
		{ name: "Apple", price: 2.58 },
        { name: "Banana", price: 1.16 },
		{ name: "Broccoli", price: 1.99 },
		{ name: "Bag Spinach(10oz)", price: 3.33 },
		{ name: "Yellow Onion", price: 0.99 },
		{ name: "Potato", price: 0.69 }
      ],
      wheat: [
		{ name: "White Bread", price: 2.99 },
		{ name: "Wheat Bread", price: 2.99 },
		{ name: "Spaghetti", price: 0.99 },
        { name: "Rice", price: 1.09 }
      ]
    },
	store3: {
      meat: [
        { name: "Chicken Breast", price: 2.99 },
        { name: "Ground Beef", price: 6.79 },
		{ name: "Ground Turkey", price: 5.29 },
		{ name: "Pork Chop", price: 7.19 },
		{ name: "Chicken Thigh", price: 3.49}
      ],
      dairy: [
		{ name: "Gallon Milk", price: 3.79 },
        { name: "Dozen Eggs", price: 8.99 },
		{ name: "Shredded Cheese(12oz)", price: 4.49 },
		{ name: "Butter (8oz)", price: 2.99 },
		{ name: "Block Cheese(8oz)", price: 2.99 }

      ],
      produce: [
		{ name: "Roma Tomato", price: 0.99 },
		{ name: "Apple", price: 1.69 },
        { name: "Banana", price: 0.65 },
		{ name: "Broccoli", price: 1.49 },
		{ name: "Bag Spinach(10oz)", price: 2.68 },
		{ name: "Yellow Onion", price: 0.89 },
		{ name: "Potato", price: 0.99 }
      ],
      wheat: [
		{ name: "White Bread", price: 2.99 },
		{ name: "Wheat Bread", price: 2.99 },
		{ name: "Spaghetti", price: 2.29 },
        { name: "Rice", price: 1.14 }
      ]
    },
	store4: {
      meat: [
        { name: "Chicken Breast", price: 6.99 },
        { name: "Ground Beef", price: 6.49 },
		{ name: "Ground Turkey", price: 4.49 },
		{ name: "Pork Chop", price: 7.99 },
		{ name: "Chicken Thigh", price: 4.99}
      ],
      dairy: [
		{ name: "Gallon Milk", price: 4.39 },
        { name: "Dozen Eggs", price: 4.99 },
		{ name: "Shredded Cheese(12oz)", price: 3.79 },
		{ name: "Butter (8oz)", price: 4.69 },
		{ name: "Block Cheese(8oz)", price: 4.99 }
      ],
      produce: [
        { name: "Roma Tomato", price: 1.16 },
		{ name: "Apple", price: 1.38 },
        { name: "Banana", price: 0.92 },
		{ name: "Broccoli", price: 1.99 },
		{ name: "Bag Spinach(10oz)", price: 2.49 },
		{ name: "Yellow Onion", price: 0.99 },
		{ name: "Potato", price: 1.58 }
      ],
      wheat: [
		{ name: "White Bread", price: 1.99 },
		{ name: "Wheat Bread", price: 2.49 },
		{ name: "Spaghetti", price: 0.99 },
        { name: "Rice", price: 1.09 }
      ]
    },
	store5: {
      meat: [
        { name: "Chicken Breast", price: 2.69 },
        { name: "Ground Beef", price: 5.99 },
		{ name: "Ground Turkey", price: 3.99 },
		{ name: "Pork Chop", price: 5.99 },
		{ name: "Chicken Thigh", price: 3.49}
      ],
      dairy: [
		{ name: "Gallon Milk", price: 4.49 },
        { name: "Dozen Eggs", price: 7.99 },
		{ name: "Shredded Cheese(12oz)", price: 2.29 },
		{ name: "Butter (8oz)", price: 1.99 },
		{ name: "Block Cheese(8oz)", price: 5.99 }
      ],
      produce: [
		{ name: "Roma Tomato", price: 1.29 },
		{ name: "Apple", price: 1.49 },
        { name: "Banana", price: 0.59 },
		{ name: "Broccoli", price: 1.49 },
		{ name: "Bag Spinach(10oz)", price: 2.29 },
		{ name: "Yellow Onion", price: 1.49 },
		{ name: "Potato", price: 0.69 }
      ],
      wheat: [
		{ name: "White Bread", price: 3.49 },
		{ name: "Wheat Bread", price: 3.29 },
		{ name: "Spaghetti", price: 1.19 },
        { name: "Rice", price: 1.25 }
      ]
    },
	store6: {
      meat: [
        { name: "Chicken Breast", price: 5.99 },
        { name: "Ground Beef", price: 8.99 },
		{ name: "Ground Turkey", price: 6.99 },
		{ name: "Pork Chop", price: 8.49 },
		{ name: "Chicken Thigh", price: 6.99}
      ],
      dairy: [
		{ name: "Gallon Milk", price: 5.99 },
        { name: "Dozen Eggs", price: 4.29 },
		{ name: "Shredded Cheese(12oz)", price: 6.49 },
		{ name: "Butter (8oz)", price: 3.99 },
		{ name: "Block Cheese(8oz)", price: 5.99 }
      ],
      produce: [
		{ name: "Roma Tomato", price: 0.99 },
		{ name: "Apple", price: 1.99 },
        { name: "Banana", price: 0.89 },
		{ name: "Broccoli", price: 1.29 },
		{ name: "Bag Spinach(10oz)", price: 2.99 },
		{ name: "Yellow Onion", price: 0.99 },
		{ name: "Potato", price: 0.99 }
      ],
      wheat: [
		{ name: "White Bread", price: 5.99 },
		{ name: "Wheat Bread", price: 5.99 },
		{ name: "Spaghetti", price: 3.19 },
        { name: "Rice", price: 1.19 }
      ]
    },
    
  };

  // Writable store for selected store
  const selectedStore = writable('');

  // Derived store for store prices
  const storePrices = derived(selectedStore, ($selectedStore) => {
    return $selectedStore ? storeData[$selectedStore] : null;
  });
</script>



<section>
	<h2>Check out products by store here!</h2>

	<p>We wanted to explore what grocery prices were like, right here in our own East Bay backyard. Right now, everything feels more expensive, and we hope that this project can provide locals with a snapshot of what their prices are doing. </p>
    
	<Image
	src="assets/images/storefront.png"
	alt="A lake and some clouds"
	
/>
    <p>In the U.S. Grocery increased 2.1% in the year of 2024. Egg prices are in the news everyday. Consumer are voicing their fears amidst looming agricultural tariffs. Everywhere people are talking about prices.</p>
    <p>So how are your prices doing?</p>
	<h1>Grocery Store Price List</h1>

<label for="store-select">Select a store:</label>
<select id="store-select" bind:value={$selectedStore}>
  <option value="">Check out a store!</option>
  <option value="store1">Whole Foods</option>
  <option value="store2">Trader Joes Berkeley</option>
  <option value="store3">Foodmaxx</option>
  <option value="store4">Trader Joes Oakland</option>
  <option value="store5">Grocery Outlet</option>
  <option value="store6">Berkeley Bowl</option>
</select>

<h2>Price Lists</h2>

{#if $storePrices}
  <div id="meat-list">
    <h3>Meat Prices</h3>
    <ul>
      {#each $storePrices.meat as item}
        <li>{item.name}: ${item.price.toFixed(2)}</li>
      {/each}
    </ul>
  </div>
  
  <div id="dairy-list">
    <h3>Dairy Prices</h3>
    <ul>
      {#each $storePrices.dairy as item}
        <li>{item.name}: ${item.price.toFixed(2)}</li>
      {/each}
    </ul>
  </div>

  <div id="produce-list">
    <h3>Produce Prices</h3>
    <ul>
      {#each $storePrices.produce as item}
        <li>{item.name}: ${item.price.toFixed(2)}</li>
      {/each}
    </ul>
  </div>

  <div id="wheat-list">
    <h3>Wheat/Grain Prices</h3>
    <ul>
      {#each $storePrices.wheat as item}
        <li>{item.name}: ${item.price.toFixed(2)}</li>
      {/each}
    </ul>
  </div>
{/if}

 
	
	<p>Meat, Produce, and Rice are priced out PER POUND, unless otherwise marked.</p>
</section>

<style>

select {
    padding: 8px;
    font-size: 1rem;
	font-family: "Quantico";
    margin-bottom: 20px;
    border-radius: 5px;
    border: 1px solid #ccc;
    width: 200px;
    display: block;
	background-color: #cf94d7;
	
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

	h2{
		font-family: "Faster One";
	}

	p{
		font-family: "Quantico";
		font-size: larger;
	}

	ul{
		display: block;
		padding-left: 5%;

	}



</style>


