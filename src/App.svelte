<script>
	import Navigation from "./components/Navigation.svelte";
	import Section from "./components/Section.svelte";
	import Footer from "./components/Footer.svelte";
</script>

<main>
	<Navigation/>
	<Section image={"/img/mars.jpeg"} title={"making life multiplanetary"} description={"SpaceX was founded under the belief that a future where humanity is out exploring the stars is fundamentally more exciting than one where we are not."} buttonText={"EXPLORE"} positionX={"left"} positionY={"center"}/>

	<Section image={"/img/rocket.jpeg"} title={"revolutionizing space technology"} description={"SpaceX’s Starship spacecraft and Super Heavy rocket is a fully reusable transportation system designed to carry both crew and cargo to Earth orbit, the Moon, Mars, and beyond."} buttonText={"LEARN MORE"} positionX={"right"} positionY={"top"}/>

	<Section image={"/img/launch.jpeg"} title={"world's leading launch service provider"} description={"SpaceX leads the world in launches with its reliable, reusable rockets and is developing the fully and rapidly reusable rockets necessary to transform humanity’s ability to access space into something as routine as air travel."} buttonText={"RESERVE YOUR RIDE"} positionX={"left"} positionY={"top"}/>

	<Section image={"/img/astronaut.jpeg"} title={"advancing human spacelight"} description={"Since returning human spaceflight capabilities to the United States in 2020, SpaceX is helping build a new era where not just hundreds of people, but thousands and ultimately millions will be able to explore space."} buttonText={"JOIN A MISSION"} positionX={"right"} positionY={"top"}/>

	<Section image={"/img/space.jpeg"} title={"delivering high-speed internet from space"} description={"Starlink is the world’s most advanced satellite constellation in low-Earth orbit, delivering reliable broadband internet capable of supporting streaming, online gaming, video calls, and more."} buttonText={"ORDER NOW"} positionX={"left"} positionY={"center"}/>

	<Footer />
</main>

<style>
	
</style>