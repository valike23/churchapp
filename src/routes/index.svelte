<script lang="ts">
	// your script goes here

	import BtmNav from "../components/BtmNav.svelte";
	let church = { name: "Deeper Life Bible Church" };
</script>

<svelte:head>
	<link
		rel="stylesheet"
		href="https://cdn.metroui.org.ua/v4/css/metro-all.min.css"
	/>
	<script src="https://cdn.metroui.org.ua/v4/js/metro.min.js" defer></script>
	<title>{church.name + " :: Home Page"}</title>
</svelte:head>

<div class="page">
	<div class="slide">
		<div id="topSlide" class="carousel slide" data-bs-ride="carousel">
			<div class="carousel-indicators">
				<button type="button" data-bs-target="#topSlide" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
				<button type="button" data-bs-target="#topSlide" data-bs-slide-to="1" aria-label="Slide 2"></button>
				<button type="button" data-bs-target="#topSlide" data-bs-slide-to="2" aria-label="Slide 3"></button>
			  </div>
			<div class="carousel-inner">
				<div class="carousel-item active">
					<img
						src="https://wallpapercave.com/wp/JUwBXRw.jpg"
						class="d-block w-100"
						style="height: 50vh"
						alt="..."
					/>
					<div class="carousel-caption ">
						<h5>First slide label</h5>
						<p>Some representative placeholder content for the first slide.</p>
					  </div>
				</div>
				<div class="carousel-item">
					<img
						src="https://wallpapercave.com/wp/NSILojy.jpg"
						class="d-block w-100"
						style="height: 50vh"
						alt="..."
					/>
					<div class="carousel-caption">
						<h5>Second slide label</h5>
						<p>Some representative placeholder content for the first slide.</p>
					  </div>
				</div>
				<div class="carousel-item">
					<img
						src="https://wallpapercave.com/wp/fq6G0ry.jpg"
						class="d-block w-100"
						style="height: 50vh"
						alt="..."
					/>
					<div class="carousel-caption">
						<h5>Third slide label</h5>
						<p>Some representative placeholder content for the first slide.</p>
					  </div>
				</div>
			</div>
			<button
				class="carousel-control-prev"
				type="button"
				data-bs-target="#topSlide"
				data-bs-slide="prev"
			>
				<span class="carousel-control-prev-icon" aria-hidden="true" />
				<span class="visually-hidden">Previous</span>
			</button>
			<button
				class="carousel-control-next"
				type="button"
				data-bs-target="#topSlide"
				data-bs-slide="next"
			>
				<span class="carousel-control-next-icon" aria-hidden="true" />
				<span class="visually-hidden">Next</span>
			</button>
		</div>
	</div>
	<!-- end Coursel -->
	
</div>
<div class="bottom">
	<BtmNav />
</div>

<style>
	.bottom {
		position: fixed;
		bottom: 0;
		left: 0;
		width: 100%;
		z-index: 100;
	}
	
</style>
