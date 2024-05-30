<script>
    import "$lib/styles/app.css"
	import Navbar from "$lib/components/Navbar.svelte";
</script>
<main>
    <Navbar></Navbar>
    <slot></slot>
</main>