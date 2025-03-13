<script>
    let choice = $state("AVG")
      $inspect({choice})
  </script>
  <div class="chart-wrapper">
    <select name="payroll years" bind:value={choice}>
        <option value="AVG">AVG</option>
        <option value="2024">2024</option>
        <option value="2023">2023</option>
         ...

    
    </select>
    
    
  {#if choice === "AVG"}
        
        <iframe title="Total Price of All Meat by Store" aria-label="Column Chart" id="datawrapper-chart-bf9kd" src="https://datawrapper.dwcdn.net/bf9kd/1/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="523" data-external="1"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"]){var e=document.querySelectorAll("iframe");for(var t in a.data["datawrapper-height"])for(var r,i=0;r=e[i];i++)if(r.contentWindow===a.source){var d=a.data["datawrapper-height"][t]+"px";r.style.height=d}}}))}();
            </script>
    
         
  {/if}
  {#if choice === "2024"}
  <iframe title="Oakland-Berkeley Grocery Stores" aria-label="Locator map" id="datawrapper-chart-G8F1m" src="https://datawrapper.dwcdn.net/G8F1m/1/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="602" data-external="1"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"]){var e=document.querySelectorAll("iframe");for(var t in a.data["datawrapper-height"])for(var r,i=0;r=e[i];i++)if(r.contentWindow===a.source){var d=a.data["datawrapper-height"][t]+"px";r.style.height=d}}}))}();
		</script>
  {/if}

</div>