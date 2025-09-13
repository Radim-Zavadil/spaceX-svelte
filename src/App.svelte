<script>
	import Navigation from "./components/Navigation.svelte";
	import Section from "./components/Section.svelte";
</script>

<main>
	<Navigation/>
	<Section image={"/img/mars.jpeg"} title={"Making life multiplanetary"} description={"SpaceX was founded under the belief that a future where humanity is out exploring the stars is fundamentally more exciting than one where we are not."} buttonText={"EXPLORE"}/>

	<Section image={"/img/rocket.jpeg"} title={"Revolutionizing space technology"} description={"SpaceX’s Starship spacecraft and Super Heavy rocket is a fully reusable transportation system designed to carry both crew and cargo to Earth orbit, the Moon, Mars, and beyond."} buttonText={"LEARN MORE"}/>
</main>

<style>
	
</style>