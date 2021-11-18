<script lang="ts">
import BtmNav from "../../components/BtmNav.svelte";
import {goto} from '@sapper/app';
import TopNav from "../../components/TopNav.svelte";

	let church = { name: "Deeper Life Bible Church" };
    const open = () =>{
        goto('donations/summary')
    }
</script>

<svelte:head>
	<link
		rel="stylesheet"
		href="https://cdn.metroui.org.ua/v4/css/metro-all.min.css"
	/>
	<script src="https://cdn.metroui.org.ua/v4/js/metro.min.js" defer></script>
	<title>{church.name + " :: Donation Page"}</title>
</svelte:head>


<div class="page ml-1">
<TopNav  header="Library"/>
<h2 class="has-header pt-4">Explore</h2>
<p>A library of resources to help you worship Jesus</p>
<br>
<div class="row" >
    <div class="cell-6 cell-sm-4" data-role="tile" data-size="medium" data-effect="hover-zoom-right">
        <div class="slide-front">
         
       <img src="images/sermon.svg" alt="sermon" class="h-100 w-100">
        </div>
        <div class="slide-back d-flex flex-justify-center flex-align-center p-4 op-mauve">
            <p class="text-center">
                Top messages
            </p>
        </div>
        <span class="branding-bar fg-dark"> Sermon</span>
    </div>
    <div class="cell-6 cell-sm-4" data-role="tile" data-size="medium" data-effect="hover-zoom-right">
        <div class="slide-front">
           
       <img src="images/sermon.svg" alt="sermon" class="h-100 w-100">
        </div>
        <div class="slide-back d-flex flex-justify-center flex-align-center p-4 op-mauve">
            <p class="text-center">
                Listen to some of the best worship songs 
            </p>
        </div>
        <span class="branding-bar fg-dark"> Worship</span>
    </div>
    <div class="cell-6 cell-sm-4" data-role="tile" data-size="medium" data-effect="hover-zoom-right">
        <div class="slide-front">
           
       <img src="images/prayer.svg" alt="sermon" class="h-100 w-100">
        </div>
        <div class="slide-back d-flex flex-justify-center flex-align-center p-4 op-mauve">
            <p class="text-center">
                Pray the right way with this solutions 
            </p>
        </div>
        <span class="branding-bar fg-white"> Guided Prayer</span>
    </div>
    <div class="cell-6 cell-sm-4" data-role="tile" data-size="medium" data-effect="hover-zoom-right">
        <div class="slide-front">
           
       <img src="images/choir.svg" alt="sermon" class="h-100 w-100">
        </div>
        <div class="slide-back d-flex flex-justify-center flex-align-center p-4 op-mauve">
            <p class="text-center">
               Daily Devotional to guide you through your daily functions
            </p>
        </div>
        <span class="branding-bar fg-white"> Daily Devotion</span>
    </div>
   
    <div class="cell-12 cell-sm-6" data-role="tile" data-size="medium" data-effect="hover-zoom-right">
        <div class="slide-front">
            <img src="images/angel.png" alt="sermon" class="h-100 w-100">
        </div>
        <div class="slide-back d-flex flex-justify-center flex-align-center p-4 op-mauve">
            <p class="text-center">
                Kids can learn using illustrative videos, books and games
            </p>
        </div>
        <span class="branding-bar fg-dark"> Kids Teaching</span>
    </div>
</div>
</div>
<div class="bottom">
	<BtmNav/>
</div>

<style>
	.bottom {
		position: fixed;
		bottom: 0;
		left: 0;
		width: 100%;
		z-index: 100;
	}
     .card-content {
       height: 20vh;

       overflow-y: scroll;
    }
    .box {
        height: 50px;
    }
	
</style>