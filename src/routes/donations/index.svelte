<script lang="ts">
	// your script goes here

import BtmNav from "../../components/BtmNav.svelte";
import TopNav from "../../components/TopNav.svelte";
import {goto} from '@sapper/app';

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

<div class="page">
<TopNav header={'Donations'}/>
<div class="row p-1">
    <div class="col">
        
<input type="text" data-role="input" placeholder="search for available donations" data-search-button="true">
    </div>
</div>
<div class="row mb-5 pb-5">
    <div class="col-12 col-sm-6 col-md-4">
        <div class="card image-header">
            <div class="card-header fg-white"
                 style="background-image: url(http://lorempixel.com/1000/600/)">
                Journey To Mountains
            </div>
            <div class="card-content p-2">
                <p class="fg-gray">Posted on January 21, 2015</p>
                Quisque eget vestibulum nulla. Quisque quis dui quis ex
                ultricies efficitur vitae non felis. Phasellus quis nibh
                hendrerit...
            </div>
            <div class="card-footer">
                <button class="button secondary">Read More</button>
            </div>
        </div>
    </div>
    <div class="col-12 col-sm-6 col-md-4">
        <div class="card image-header">
            <div class="card-header fg-white"
                 style="background-image: url(http://lorempixel.com/1000/600/)">
                Church Tithe
            </div>
            <div class="card-content p-2">
                <p class="fg-gray">Posted on January 21, 2015</p>
                Tithe is 10% of your gross income and earning.
                 Abraham gave tithes to Melchisedec, king of Salem, 
                 but this was the spoils of war, not the legalistic tithe
                  of the land which Moses commanded. Also, God did not
                   command the tithe, Abraham chose to give it of his 
                   own free will (Genesis 14:17-23; Hebrews 7:1-10). 
                   The only other
                 scriptural reference to tithing before Moses is Jacob.
            </div>
            <div class="card-footer">
                <button on:click="{()=>{open()}}" class="button secondary">GIVE</button>
            </div>
        </div>
    </div>
    <div class="col-12 col-sm-6 col-md-4">
        <div class="card image-header">
            <div class="card-header fg-white"
                 style="background-image: url(http://lorempixel.com/1000/600/)">
                Journey To Mountains
            </div>
            <div class="card-content p-2">
                <p class="fg-gray">Posted on January 21, 2015</p>
                Quisque eget vestibulum nulla. Quisque quis dui quis ex
                ultricies efficitur vitae non felis. Phasellus quis nibh
                hendrerit...
            </div>
            <div class="card-footer">
                <button class="button secondary">Read More</button>
            </div>
        </div>
    </div>
    <div class="col-12 col-sm-6 col-md-4">
        <div class="card image-header">
            <div class="card-header fg-white"
                 style="background-image: url(http://lorempixel.com/1000/600/)">
                Journey To Mountains
            </div>
            <div class="card-content p-2">
                <p class="fg-gray">Posted on January 21, 2015</p>
                Quisque eget vestibulum nulla. Quisque quis dui quis ex
                ultricies efficitur vitae non felis. Phasellus quis nibh
                hendrerit...
            </div>
            <div class="card-footer">
                <button class="button secondary">Read More</button>
            </div>
        </div>
    </div>
    <div class="col-12 col-sm-6 col-md-4">
        <div class="card image-header">
            <div class="card-header fg-white"
                 style="background-image: url(http://lorempixel.com/1000/600/)">
                Journey To Mountains
            </div>
            <div class="card-content p-2">
                <p class="fg-gray">Posted on January 21, 2015</p>
                Quisque eget vestibulum nulla. Quisque quis dui quis ex
                ultricies efficitur vitae non felis. Phasellus quis nibh
                hendrerit...
            </div>
            <div class="card-footer">
                <button class="button secondary">Read More</button>
            </div>
        </div>
    </div>
    <div class="col-12 col-sm-6 col-md-4">
        <div class="card image-header">
            <div class="card-header fg-white"
                 style="background-image: url(http://lorempixel.com/1000/600/)">
                Journey To Mountains
            </div>
            <div class="card-content p-2">
                <p class="fg-gray">Posted on January 21, 2015</p>
                Quisque eget vestibulum nulla. Quisque quis dui quis ex
                ultricies efficitur vitae non felis. Phasellus quis nibh
                hendrerit...
            </div>
            <div class="card-footer">
                <button class="button secondary">Read More</button>
            </div>
        </div>
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
	
</style>
