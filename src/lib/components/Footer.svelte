<script>
    import Logo from "./Logo.svelte";
	import { Icon } from "svelte-icons-pack";
	import {
		RiLogosDiscordFill,
		RiLogosInstagramFill,
	} from "svelte-icons-pack/ri";
</script>
<footer>
    <a href="../"> <Logo width="25"></Logo></a>
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
    <p>
        &copy; dazon {`${new Date().getFullYear()}`}
    </p>
</footer>

<style>
    p {
        width: fit-content !important;
        margin: 0 !important;
    }
</style>