// Store price data
<script>
const storeData = {
    wholeFoods: {
        meat: [
            { name: "Chicken", price: 5.99 },
            { name: "Beef", price: 8.99 },
        ],
        dairy: [
            { name: "Milk", price: 2.99 },
            { name: "Cheese", price: 4.49 },
        ],
        produce: [
            { name: "Apple", price: 1.99 },
            { name: "Banana", price: 0.99 },
        ],
        wheat: [
            { name: "Bread", price: 2.49 },
            { name: "Pasta", price: 1.99 },
        ]
    },
    tjBerk: {
        meat: [
            { name: "Chicken", price: 6.49 },
            { name: "Pork", price: 7.99 },
        ],
        dairy: [
            { name: "Milk", price: 3.19 },
            { name: "Butter", price: 2.99 },
        ],
        produce: [
            { name: "Tomato", price: 2.49 },
            { name: "Lettuce", price: 1.29 },
        ],
        wheat: [
            { name: "Bread", price: 3.19 },
            { name: "Cereal", price: 2.89 },
        ]
    },
    foodMaxx: {
        meat: [
            { name: "Chicken", price: 6.49 },
            { name: "Pork", price: 7.99 },
        ],
        dairy: [
            { name: "Milk", price: 3.19 },
            { name: "Butter", price: 2.99 },
        ],
        produce: [
            { name: "Tomato", price: 2.49 },
            { name: "Lettuce", price: 1.29 },
        ],
        wheat: [
            { name: "Bread", price: 3.19 },
            { name: "Cereal", price: 2.89 },
        ]
    },
    tjOak: {
        meat: [
            { name: "Chicken", price: 6.49 },
            { name: "Pork", price: 7.99 },
        ],
        dairy: [
            { name: "Milk", price: 3.19 },
            { name: "Butter", price: 2.99 },
        ],
        produce: [
            { name: "Tomato", price: 2.49 },
            { name: "Lettuce", price: 1.29 },
        ],
        wheat: [
            { name: "Bread", price: 3.19 },
            { name: "Cereal", price: 2.89 },
        ]
    },
    gOutlet: {
        meat: [
            { name: "Chicken", price: 6.49 },
            { name: "Pork", price: 7.99 },
        ],
        dairy: [
            { name: "Milk", price: 3.19 },
            { name: "Butter", price: 2.99 },
        ],
        produce: [
            { name: "Tomato", price: 2.49 },
            { name: "Lettuce", price: 1.29 },
        ],
        wheat: [
            { name: "Bread", price: 3.19 },
            { name: "Cereal", price: 2.89 },
        ]
    },
    berkBowl: {
        meat: [
            { name: "Chicken", price: 6.49 },
            { name: "Pork", price: 7.99 },
        ],
        dairy: [
            { name: "Milk", price: 3.19 },
            { name: "Butter", price: 2.99 },
        ],
        produce: [
            { name: "Tomato", price: 2.49 },
            { name: "Lettuce", price: 1.29 },
        ],
        wheat: [
            { name: "Bread", price: 3.19 },
            { name: "Cereal", price: 2.89 },
        ]
    },
    // Repeat for other stores (store3, store4, etc.)
};

// Function to update price lists
function updatePriceLists(store) {
    // Check if store exists in the storeData object
    if (!storeData[store]) return;

    // Get the price data for the selected store
    const storePrices = storeData[store];

    // Update the meat prices
    const meatList = document.querySelector("#meat-list ul");
    meatList.innerHTML = storePrices.meat.map(item => `<li>${item.name}: $${item.price.toFixed(2)}</li>`).join("");

    // Update the dairy prices
    const dairyList = document.querySelector("#dairy-list ul");
    dairyList.innerHTML = storePrices.dairy.map(item => `<li>${item.name}: $${item.price.toFixed(2)}</li>`).join("");

    // Update the produce prices
    const produceList = document.querySelector("#produce-list ul");
    produceList.innerHTML = storePrices.produce.map(item => `<li>${item.name}: $${item.price.toFixed(2)}</li>`).join("");

    // Update the wheat/grain prices
    const wheatList = document.querySelector("#wheat-list ul");
    wheatList.innerHTML = storePrices.wheat.map(item => `<li>${item.name}: $${item.price.toFixed(2)}</li>`).join("");
}

// Event listener for store selection
document.getElementById("store-select").addEventListener("change", function() {
    const selectedStore = this.value;
    updatePriceLists(selectedStore);
});

</script>