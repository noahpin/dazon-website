<script>
	export let imageSource;
	export let headerText = null;
	export let headerClass = "";
	export let heightOverride = null;
	export let noHover = false;
	import GbStatus from "./GBStatus.svelte";
	export let status = null;
	export let customStatus = null;
	export let forceView = false;
</script>

<div
	class={"header-image-wrap " + (forceView ? "viewt" : "")}
	style={heightOverride ? `height: ${heightOverride};` : ""}
>
	{#if !noHover}
		<img class={"blur-image hover-image"} src={imageSource} alt="" />
	{/if}
	<div class="header-image">
		<img src={imageSource} alt="" />
		{#if headerText != null}
		<img class="blur-image" src={imageSource} alt="" />
		{/if}
	</div>
	{#if headerText != null}
	<div class="bar">
		<h1 class={headerClass}>{headerText}</h1>
		{#if status != null}
			<GbStatus {status} {customStatus}></GbStatus>
		{/if}
	</div>
	{/if}
</div>

<style>
	.header-image-wrap {
		width: 100%;
		height: min(470px, 65vh);
		position: relative;
		flex-shrink: 1;
	}
	.viewt {
		view-transition-name: header-image;
	}
	.header-image {
		width: 100%;
		height: 100%;
		position: relative;
		overflow: hidden;
		border-radius: 10px !important;
		border: 1px solid rgba(255, 255, 255, 0.14);
	}
	.header-image img {
		width: 100%;
		height: 100%;
		position: absolute;
		object-fit: cover;
		padding: 0;
		display: block;
	}
	.header-image-wrap h1 {
		margin: 0;
		font-size: 60px;
	}
	.blur-image {
		--blursize: 10px;

		filter: blur(var(--blursize)) contrast(200%) brightness(0.4);
		width: calc(100% + var(--blursize) * 2) !important;
		height: calc(100% + var(--blursize) * 2) !important;
		transform: translate(
			calc(var(--blursize) * -1),
			calc(var(--blursize) * -1)
		);
		mask-image: linear-gradient(
			to bottom,
			transparent calc(100% - 220px),
			black
		);
	}
	.bar {
		margin: 20px 30px;
		width: auto;
		left: 0px;
		right: 0px;
		max-width: 100%;
		padding-bottom: 10px;
		position: absolute;
		bottom: 0;
		left: 0;
		align-items: center;
		display: flex;
		justify-content: space-between;
		gap: 20px;
		flex-wrap: wrap;
	}
	.hover-image {
		--blursize: 0px;
		width: 100% !important;
		height: 100% !important;
		transform: none !important;
		position: absolute;
		object-fit: cover;
		padding: 0;
		display: block;
		top: 0px;
		mask-image: none;
		opacity: 0;
		transition: 0.5s;
	}
	.header-image-wrap:hover .hover-image {
		opacity: 0.41;
		--blursize: 25px;
		top: 5px;
		filter: blur(var(--blursize)) contrast(200%) brightness(2);
	}
</style>
