<script>
    import Image from "./helpers/Image.svelte";
</script>
<section>
	<h2>The Reflection</h2>

    <p>Throughout the process of exploring this topic, we realized there were only so many things we could achieve.</p>    
    <p>Let’s take a look at where we fell short.  In its beginning, this project had hoped to showcase the changes of food prices over time, an idea that was sparked by the White House announcing a plan to place 25% tariffs on Canada and Mexico, but during our time that tariff was never put into effect. </p>
    <p>After that, we saw this project as a chance to take a deeper look into food prices as they were, and give consumers a little help with navigating the madness that exists in the vacuum of options that exist today. </p>
    <p>Despite our careful analysis and best intentions, there were a few roadblocks.</p>
    <p>The first was price gathering. We visited during a three day stretch all 6 of our stores to collect the data for this project. One immediate downside to this is that grocery store prices change day to day, even throughout the day in many cases. Another issue was to decide what prices to pick. </p>
    <p>We decided to focus on the cheapest goods we could find, that were not organic, in order to remain consistent at each store. The drawback to that is potentially our analysis on the quality of certain products. </p>
    <p>For example, in Whole Foods and Berkeley Bowl, many parts of the store default to organic products, as they are trying to specialize in those products specifically, more than they are trying to sell the cheapest goods they possibly can. That choice may make their non-organic products slightly more expensive than other stores, while simultaneously having cheaper organic options than other stores may have.</p>
    <p>The second was calculations. In some cases we listed food by weight to keep our data consistent, yet certain stores sell products, particularly produce, by item, not by pound. An example of this is Trader Joe’s, where a yellow onion costs about $0.99 per onion, instead of listing its price per pound. In the data, we researched the weight of a typical Trader Joe’s Yellow onion and found it to be about 1 lb, so we simply kept the price of $0.99 per pound to represent their onions. Overall, the process did not create any stark outliers, but it is a part of the imperfections in our method.</p>
    <p>Finally, we saw that occasionally stores were out of stock of items, but still had the price labels for those missing products. The biggest example was eggs.</p>
    <p>At Whole Foods, we saw this first hand. </p>

    <div class="small">
        <Image
            src="assets/images/noeggs.jpg"
            alt="A lake and some clouds"
            caption="An empty refrigerator Section at Whole Foods, Berkeley."
            
        />
    </div>

    <p>On this occasion, we returned to the store to see if the missing product had been replaced, and upon returning the next day, Whole Foods had indeed restocked its egg supply. Even in doing so, it is worth noting that each store we visited had very low egg supplies, even if their prices were reasonably unchanged. 
    </p>


    <h2>Final Thoughts</h2>

    <p>We hope that this project can be helpful for all the Oakland/Berkeley shoppers out there, and we hope it gives people an easy way to explore what each store may have to offer, without diving too far into the madness themselves. </p>
    <p>We also hope that everyone takes this opportunity to reflect on what this project is not: A full, in-depth, complete scope of the grocery posibilities in the East Bay, but instead a window into what already exists, a few places at a time.</p>
   
	
	<p>We hope you enjoyed.</p>
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

	h2{
		font-family: "Faster One";
	}

	p{
		font-family: "Quantico";
		font-size: larger;
	}

    .small {
		width: 400px;
		margin: 5px auto;
        
	}

</style>