<script>
    import Image from "./helpers/Image.svelte";
</script>
<section>
	<h2>The Analysis</h2>
   
    <p>In this section, we are going through the data we collected in hopes of providing a better explanation of what these numbers could mean, as well as examining any trends we thought were interesting.</p>
    <p>We'll start by looking at how meat prices compare from each of our stores, with a comparison of their Total Price.</p>
   

    <div class="graphic">
        <iframe title="Total Price of All Meat by Store" aria-label="Column Chart" id="datawrapper-chart-bf9kd" src="https://datawrapper.dwcdn.net/bf9kd/1/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="523" data-external="1"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"]){var e=document.querySelectorAll("iframe");for(var t in a.data["datawrapper-height"])for(var r,i=0;r=e[i];i++)if(r.contentWindow===a.source){var d=a.data["datawrapper-height"][t]+"px";r.style.height=d}}}))}();
        </script>
    </div>

    <p>Looking at the graph, the cheapest 2 stores we found were from Oakland, with the two Trader Joe's tying for thrid place, and Berkeley Bowl taking last place. </p>
    <p>There was only about a $15 dollar gap between our cheapest and our most expensive store. Yet, within <strong>both</strong> cities, that same gap shrunk to about $7 in berkeley and $8 in Oakland. </p>
    <p>The greatest explanation we could see for the diferences was in the price per pound of Chicken. Both Chicken Breast and Chicken Thighs were significatly cheaper in Grocery Outlet and in Foodmaxx, when compared to the Berkeley Grocery Stores options for the same products.</p>

    <div class="small">
        <Image
            src="assets/images/meat.png"
            alt="A lake and some clouds"
            
        />
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

    .graphic {
        background-color: #fedcdc;
        margin-left: 5px;
        margin-right: 5px;
        padding: 2%;
        border-radius: 8px;
     
    }

    h2, p{
        text-align: center;
    }

	h2{
		font-family: "Faster One";
	}

	p{
		font-family: "Quantico";
	}

    .small {
		width: 175px;
		margin: 15px auto;
	}

</style>




