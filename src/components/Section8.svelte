<script>
    import Image from "./helpers/Image.svelte";
</script>

<section>
	<h2>EGGS</h2>
   
    <h3>So let's talk about <strong>eggs.</strong></h3>
    <p>Expensive and troublesome to find, eggs have become a luxury item in the last few months due to an outbreak of bird flu that has caused prices to soar. The bird flu outbreak began in the U.S in 2022; since then, over 163 million chickens, turkeys, and other poultry birds have died. With the number of egg-laying birds massively depleted, egg supplies have been estimated to have decreased by 40% compared to last year. As a result, prices are almost double what they were in 2024. </p>
    <p>And we could see the effects in our findings:</p>

    <div class="graphic">
        <iframe title="An Egg-Price Comparison in the East Bay" aria-label="Bar Chart" id="datawrapper-chart-3V7cE" src="https://datawrapper.dwcdn.net/3V7cE/1/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="296" data-external="1"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"]){var e=document.querySelectorAll("iframe");for(var t in a.data["datawrapper-height"])for(var r,i=0;r=e[i];i++)if(r.contentWindow===a.source){var d=a.data["datawrapper-height"][t]+"px";r.style.height=d}}}))}();
        </script>
    </div>

    <p> While overall dairy products were lower at Foodmaxx and Grocery Outlet, both stores had much higher prices for a dozen eggs, with eggs being $7.99 at Grocery Outlet and $8.99 at Foodmaxx. To contrast, smaller-scale stores like Trader Joe’s have managed to keep a dozen eggs under $5. </p>
    <p>According to CNBC Make It, Trader Joe’s prevents their prices from spiking as they buy directly from suppliers as well as using private-label brands. This means that they avoid price markups, maintaining more control over costs. Trader Joe’s also recently put a limit on the number of eggs shoppers were able to purchase, limiting it to one dozen per customer to manage their limited supply. 
    </p>

    <div class="small">
        <Image
            src="assets/images/eggs.png"
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

    h2, p, h3{
        text-align: center;
    }

	h2{
		font-family: "Faster One";
	}

	p, h3{
		font-family: "Quantico";
	}

    .small {
		width: 175px;
		margin: 15px auto;
	}

</style>




