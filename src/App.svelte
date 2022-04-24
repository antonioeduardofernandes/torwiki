<script>
	// import { onMount } from "svelte";
	// import { gsap } from "gsap";
	// import { ScrollTrigger } from "gsap/ScrollTrigger";
	// gsap.registerPlugin(ScrollTrigger);
	// import Scrollbar from "smooth-scrollbar";

	// loads wind sound opening
	// import mainaudio from "./scripts/mainaudio";

	//import Components
	import Topbar from "./components/Topbar/Topbar.svelte";
	import CharacterCard from "./components/Cards/CharacterCard.svelte";
	import OverlayMenu from "./components/Topbar/OverlayMenu.svelte"
</script>

<main>
	<Topbar />
	<OverlayMenu/>
	<div class="content">
		<CharacterCard />
	</div>
</main>

<style>
	@font-face {
		font-family: "Flareserif";
		src: url("/fonts/Flareserif.ttf");
	}

	:global(body) {
		position: relative;
		padding: 0;
		margin: 0;
		box-sizing: border-box;
		background-color: #131313;
		color: rgb(177, 177, 177);
		font-family: "Flareserif", serif;
		letter-spacing: 2px;
	}
</style>
