<script>
    import Home from "../components/home.svelte";
    import About from "../components/about.svelte";
    import Projects from "../components/projects.svelte"
    import Contacts from "../components/contacts.svelte";
    import "../global.css";

    import { onMount } from "svelte";
	import VanillaTilt from "vanilla-tilt";

	onMount(() => {
		const elements = document.querySelectorAll("[data-tilt]");
		VanillaTilt.init(elements, {
			max: 10, // sesuai data-tilt-max="5" kamu
			scale: 1, // sesuai data-tilt-scale="1" kamu
			reverse: false,
		});
	});
	let { children } = $props();
</script>

    <Home>
    
</Home>
<About>
</About>
<Projects></Projects>
<Contacts></Contacts>