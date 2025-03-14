
	  <!-- Section to display products based on the selected store -->
	  <div id="productList"></div>
	
	  <script>
		// Define the stores and their products
		const stores = {
		  store1: [
			{ name: "Apple", price: 1.2 },
			{ name: "Banana", price: 0.5 }
		  ],
		  store2: [
			{ name: "Apple", price: 1.3 },
			{ name: "Carrot", price: 0.8 }
		  ],
		  store3: [
			{ name: "Apple", price: 1.1 },
			{ name: "Banana", price: 0.6 },
			{ name: "Carrot", price: 0.9 }
		  ]
		};
	
		// Function to render the products of the selected store
		function renderProducts(store) {
		  const productListDiv = document.getElementById('productList');
		  productListDiv.innerHTML = ''; // Clear the existing products
	
		  if (store) {
			const products = stores[store];
			let productHtml = `<h3>Products at ${store}</h3><ul>`;
			products.forEach(product => {
			  productHtml += `<li>${product.name}: $${product.price}</li>`;
			});
			productHtml += '</ul>';
			productListDiv.innerHTML = productHtml;
		  } else {
			productListDiv.innerHTML = '<p>Please select a store to view products.</p>';
		  }
		}
	
		// Get the dropdown menu element and add an event listener for changes
		const storeDropdown = document.getElementById('storeDropdown');
		storeDropdown.addEventListener('change', (event) => {
		  const selectedStore = event.target.value;
		  renderProducts(selectedStore);
		});
	
	  </script>
    