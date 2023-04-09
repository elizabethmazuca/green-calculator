<script>
	const snackMap = {
		'Fruit Snacks': 0,
		'Plastic Bottle': 0,
		'Aluminum Can': 0,
		'Chip Bag': 0
	};
	function incrementSnack(snackName) {
		snackMap[snackName]++;
	}
	function incrementFruitSnack() {
		incrementSnack('Fruit Snacks');
	}

	function incrementPlasticBottle() {
		incrementSnack('Plastic Bottle');
	}

	function incrementAluminumCan() {
		incrementSnack('Aluminum Can');
	}

	function incrementChipBag() {
		incrementSnack('Chip Bag');
	}
</script>

<div class="container">
	<ul class="nav">
		<li>
			<a class="navlink" href="/">Home</a>
		</li>
		<li>
			<a class="navlink" href="page1.html">Page 1</a>
		</li>
		<li>
			<a class="navlink" href="page2.html"> Page 2</a>
		</li>
	</ul>
	<h1 class="title">Plastic Decomposition Facts</h1>
	<p class="pictureCaption">Here's a picture of our contaminated ocean</p>
	<div>
		<img class="oceantrash" src="./assets/oceantrash.png" alt="Ocean Trash" />
	</div>

	<!-- function increment () 
    {
        count = 0
        $count++;
    } -->

	<!-- SAD PLASTIC FACTS-->

	<!-- <h1 class="pictureCaption">Did you know</h1>
	<br />
	<p class="pictureCaption">
		It takes 450 years to decompose a water bottle. <br /> It takes 80-200 years to decompose an
		aluminum can.
		<br /> It takes 10-20 years to decompose a chip bag.
	</p> -->

	<table align="center">
		<tr>
			<td> It takes 450 years to decompose a water bottle. </td>
			<td>It takes 80-200 years to decompose an aluminum can.</td>
			<td> It takes 10-20 years to decompose a chip bag. </td>
		</tr>
	</table>

	<!-- SNACK BUTTONS -->
	<br /> <button on:click={incrementFruitSnack}> Fruit Snacks {snackMap['Fruit Snacks']}</button>
	<br /> <br />
	<button on:click={incrementPlasticBottle}> Plastic Bottle {snackMap['Plastic Bottle']} </button>
	<br /> <br />
	<button on:click={incrementAluminumCan}> Aluminum Can {snackMap['Aluminum Can']} </button> <br />
	<br />
	<button on:click={incrementChipBag}> Chip Bag {snackMap['Chip Bag']}</button>
</div>

<style>
	h1 {
		color: green;
		text-align: center;
	}

	p {
		text-align: center;
		font-size: 24pt;
	}
	div {
		text-align: center;
	}
	td {
		padding: 70px;
		width: 13ch;
		font-size: 24pt;
	}
</style>
