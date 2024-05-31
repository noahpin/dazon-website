<script>
	import Logo from "$lib/components/Logo.svelte";
	import { page } from "$app/stores";
	import { Icon } from "svelte-icons-pack";
	import {
		RiLogosDiscordFill,
		RiLogosInstagramFill,
	} from "svelte-icons-pack/ri";
	$: console.log($page.url.pathname);
</script>

<div class="navbar">
	<div class="navbar-inner">
		<a href="../"> <Logo width="25"></Logo></a>
		<a href="../" class={$page.url.pathname == "/" ? "active" : ""}>projects</a>
		<a href="../about" class={$page.url.pathname == "/about" ? "active" : ""}
			>about</a
		>
		<a href="https://discord.dazon.xyz/" target="_blank"
			><Icon
				src={RiLogosDiscordFill}
				size="28"
			/>
		</a>
		<a href="https://www.instagram.com/dazon.mk/" target="_blank"
			><Icon
				src={RiLogosInstagramFill}
				size="28"
			/></a
		>
	</div>
</div>

<style>
</style>
