<script lang="ts">
    import BtmNav from "../../components/BtmNav.svelte";
    import TopNav from "../../components/TopNav.svelte";
    let amount = 0;
    const increaseAmount = (money) =>{
        amount += money;
    }
</script>

<svelte:head>
    <link
        rel="stylesheet"
        href="https://cdn.metroui.org.ua/v4/css/metro-all.min.css"
    />
    <script src="https://cdn.metroui.org.ua/v4/js/metro.min.js" defer></script>
    <title>Donation: Summary</title>
</svelte:head>
<div class="page mb-5">
    <TopNav header={"Donation Summary"} />
    <div class="row mt-5">
        <div class="col">
            <div
                style="background-image: url(http://lorempixel.com/1000/600/)"
                class="jumbotron jumbotron-fluid "
            >
                <div class="container">
                    <h1 class="display-4">Fluid jumbotron</h1>
                    <p class="lead">
                        This is a modified jumbotron that occupies the entire
                        horizontal space of its parent.
                    </p>
                </div>
            </div>
        </div>
    </div>
</div>
<div class="row">
    <div class="col-12 d-flex flex-wrap align-content-center">
        <div id="amountCon">
            <span id="naira"> ₦</span>
            <input class="text-center" size="50" id="amount" bind:value="{amount}" type="number" >
        </div>
    </div>
    <div class="col-12 mt-3">
        <div class="money">
            <div data-role="buttongroup" class="">
                <button on:click="{()=>{increaseAmount(5)}}"  class="button bg-brown fg-white"> ₦5</button>
                <button on:click="{()=>{increaseAmount(10)}}" class="button bg-yellow fg-white">₦10</button>
                <button on:click="{()=>{increaseAmount(20)}}" class="button bg-green fg-white">₦20</button>
                <button on:click="{()=>{increaseAmount(50)}}" class="button bg-blue fg-white">₦50</button>
                <button on:click="{()=>{increaseAmount(100)}}" class="button bg-amber fg-white">₦100</button> 
                <button on:click="{()=>{increaseAmount(200)}}" class="button bg-lime fg-white">₦200</button>
                <button on:click="{()=>{increaseAmount(500)}}" class="button bg-red ribbed-orange fg-white ">₦500</button>
                <button on:click="{()=>{increaseAmount(1000)}}" class="button bg-gray fg-white">₦100</button>
            </div>
        </div>
    </div>
   
    <div class="col-12 money mt-5">
        
<button style="min-width: 200px;"  class="button primary large">Pay</button>
    </div>
</div>

<div class="bottom">
    <BtmNav />
</div>

<style>
    #amountCon {
        margin-left: 25vw;
    }
    #amount {
        width: 50vw;
        height: 150px;
        border: 0;
        font-size: 70px;
        background-color: whitesmoke;
       
    }
    #naira {
        font-size: 30px;
        margin-left: -25px;
    }
    .money {
        display: flex;
     justify-content: center;
    }
    .bottom {
        position: fixed;
        bottom: 0;
        left: 0;
        width: 100%;
        z-index: 100;
    }
    .jumbotron {
        height: 30vh;
        padding-top: 6vh;
    }
</style>
