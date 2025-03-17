<script>
    import Image from "./helpers/Image.svelte";
</script>
<section>
	<h2>The Produce</h2>
   
    <p>In today's world, finding fruits and vegetables is hardly a challenge, they're readily available at local grocery stores, farmers' markets, and even convenience stores. However, the true challenge lies in finding produce that meets the standards of quality many consumers are looking for and want. </p>
    <p>High-quality fruits and vegetables, often grown without harmful pesticides or with sustainable practices, may not be as easily accessible in every store. And when you do find them, they tend to come with a higher price tag.</p>
    <p>Here, we have all of our produce products compared so that shoppers can easily compare directly each of these products by price, and see what differences stand out to them.</p>

    <div class="graphic">
        <iframe title="Comparing All Produce Products" aria-label="Multiple Columns" id="datawrapper-chart-gEOQS" src="https://datawrapper.dwcdn.net/gEOQS/1/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="652" data-external="1"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"]){var e=document.querySelectorAll("iframe");for(var t in a.data["datawrapper-height"])for(var r,i=0;r=e[i];i++)if(r.contentWindow===a.source){var d=a.data["datawrapper-height"][t]+"px";r.style.height=d}}}))}();
        </script>
    </div>

    <p>Looking at the graph, Whole Foods appears to be an outlier. It stands tall above the rest, but the reason for that may be because Whole Foods specializes in Organic produce. </p>
    <p>At all the Grocery Stores we examined, we took the non-organic options for our product baskets. This in turn may lead to some stores, such as Whole Foods, appearing much more expensive than they actually are. </p>
    <p>This is where specialty stores like Berkeley Bowl stand out. Known for their incredible variety of fresh, high-quality produce, Berkeley Bowl prioritizes sourcing from local farmers and offering organic, non-GMO, and sustainably grown options, and it's still pretty cheap. </p>
    <p>We spoke to Economist Dan Lindheim about what he thought of the local prices:</p>
  
    <p id="quote">“Well, Berkeley bowl is not cheap, let's just be real. Berkeley bowl has incredible variety. It has incredible opportunities to buy lots of different things. Especially, if you know, fruits and vegetables, meat, things like that, but it's more of a quality store that isn't an expensive store.”</p>

    <p>Berkeley Bowl ranked third in our Produce rankings, only $0.80 away from the cheapest store, Grocery Outlet. In our analysis, this category was more difficult to examine than the other three. For the most part that difficulty came from the variety of produce we found at each store. We found it hard to fairly compare the stores when we knew that each one chose to specialize in produce differently. But we wanted to share our findings either way.</p>

    <div class="small">
        <Image
            src="assets/images/onion.png"
            alt="A lake and some clouds"
            
        />
    </div>

</section>

<style>

.small {
		width: 175px;
		margin: 15px auto;
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

    #quote{
        font-size: x-large;
        font-weight: bolder;
        word-spacing: 10%;
    }

</style>