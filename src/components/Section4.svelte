<script>
	import Image from "$components/helpers/Image.svelte";

   
</script>

<section>
	<h2>The Method</h2>

    <p>We wanted to look at six Oakland/Berkeley Grocery Stores to see what food prices were like right now for shoppers. This is where we looked:</p>    
    

	<div class="map">
		
		<iframe title="Oakland-Berkeley Grocery Stores" aria-label="Locator map" id="datawrapper-chart-G8F1m" src="https://datawrapper.dwcdn.net/G8F1m/1/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="602" data-external="1"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"]){var e=document.querySelectorAll("iframe");for(var t in a.data["datawrapper-height"])for(var r,i=0;r=e[i];i++)if(r.contentWindow===a.source){var d=a.data["datawrapper-height"][t]+"px";r.style.height=d}}}))}();
		</script>
	
	</div>
	
    
    <p>Our goal was to select stores that were spread out geographically, in hopes of representing as many different neighborhoods as we could with such a limited amount of stores.</p>

	<p>We also selected one Trader Joes in Berkeley and one in Oakland to try and see if there was any stark differrence between two grocery stores of the same parent company.</p>

	

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

	.map {
		background: #FFEAEA;
		max-width: 600px;
		margin: 20px auto;
		padding: 10px;
		border-radius: 10px;
		
      
      
	}



</style>