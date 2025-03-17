<script>
    import Image from "./helpers/Image.svelte";
</script>
<section>
	<h2>The Wheat & Grains</h2>
   
    <p>We should just call this one bread, rice, and pasta. Because that's what we looked at.</p>
   

    <div class="graphic">
        <iframe title="Comparing Wheat &amp;amp; Grain Prices by Product" aria-label="Split Bars" id="datawrapper-chart-FBV7G" src="https://datawrapper.dwcdn.net/FBV7G/1/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="255" data-external="1"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"]){var e=document.querySelectorAll("iframe");for(var t in a.data["datawrapper-height"])for(var r,i=0;r=e[i];i++)if(r.contentWindow===a.source){var d=a.data["datawrapper-height"][t]+"px";r.style.height=d}}}))}();
        </script>
    </div>

    <p>Bread is one of the most common food items. In the year 2020, 327 million Americans reported using bread, The data has been calculated by Statista based on the U.S. Census data and Simmons National Consumer Survey (NHCS).</p>
   
    <p>Overall, bread prices we decently consistant, with about a $2 dollar gap between are cheapest and our second-most expensive store. The exception was at the Berkeley Bowl. When colelcting our data, we noticed that Berkeley Bowl Bread was consistently being sold at $5.99 or more, which causes it to stand out when looking at our stores total prices for Wheat & Grain products. </p>
    <p>On the other end, Trader Joe's Oakland was a superstar in this category. It ranked first or tied-for first for each of our prodcuts here, making it the resounding choice for cheap products in this category, based on the stores selected. </p>


    <div class="small">
        <Image
            src="assets/images/bread.png"
            alt="A lake and some clouds"
            
        />
    </div>

</section>

<style>

.small {
		width: 200px;
		margin: 5px auto;
	}

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

</style>
