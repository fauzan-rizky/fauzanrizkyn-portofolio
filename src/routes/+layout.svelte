<script>
	import favicon from "$lib/assets/favicon.svg";
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

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}
