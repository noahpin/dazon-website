<script>
	import ProjectImage from "$lib/components/ProjectImage.svelte";
	import Keyreative from "$lib/assets/logos/keyreative.png";
	import Cannonkeys from "$lib/assets/logos/cannonkeys.png";
	import Deskhero from "$lib/assets/logos/deskhero.png";
	import Ilumkb from "$lib/assets/logos/ilumkb.png";
	import Keebzncables from "$lib/assets/logos/keebzncables.png";
	import Keygem from "$lib/assets/logos/keygem.png";
	import Prototypist from "$lib/assets/logos/prototypist.png";
	import Zfrontier from "$lib/assets/logos/zfrontier.png";
	import D from "$lib/components/D.svelte";
	import CircleSix from "$lib/components/CircleSix.svelte";
	import SeventhLogo from "$lib/components/SeventhLogo.svelte";

	var heightOverride = "min(300px, 65vh)";
</script>

<div class="fullpage-wrapper">
	<div class="fullpage">
		<ProjectImage
			noHover={true}
			imageSource={"https://i.imgur.com/Xgtnxdd.jpeg"}
			heightOverride={"100%"}
			headerClass={"astha-header"}
			headerText={"KAM ASTHA"}
			status={"ic"}
			customStatus={"Group Buy May 31st"}
			forceView={true}
		></ProjectImage>
	</div>
</div>
<p>
	IN ANOTHER UNIVERSE, NOT TOO DISSIMILAR FROM OURS, THERE EXISTS THE PLANET
	&lt;ASTHA&gt;. TO LEARN ABOUT THEM, WE MUST COMMUNICATE. TO COMMUNICATE, WE
	MUST BE ABLE TO TYPE.
	<br /><br />
	THIS KEYCAP SET IS A MANIFESTATION OF THE &lt;ASTHAN&gt; LANGUAGE, ADAPTED FOR
	SIMPLE ENGLISH TRANSLATION.
	<br /><br />
	USE THEM WITH IMPORTANCE. GAIN THEIR WISDOM.
</p>
<h1>details</h1>
<p>
	<span>GROUP BUY: MAY 31ST - JULY 1ST</span><D /><span
		>PROFILE: KEYREATIVE KAM</span
	>
	<D /><span>MATERIAL: PBT DYE-SUBLIMATION</span><D /><span>TEXTURE: MATTE</span
	>
</p>
<h1>Vendors</h1>
<div class="vendor-wrapper">
	<a
		href="https://cannonkeys.com/products/kam-astha"
		target="_blank"
		class="vendor-card"
	>
		<p>us:</p>
		<img src={Cannonkeys} alt="" />
	</a>
	<a
		href="https://www.deskhero.ca/products/kam-astha-keycaps-group-buy"
		target="_blank"
		class="vendor-card"
	>
		<p>ca:</p>
		<img src={Deskhero} alt="" />
	</a>
	<a
		href="https://keygem.com/products/kam-astha-keycaps-group-buy"
		target="_blank"
		class="vendor-card"
	>
		<p>eu:</p>
		<img src={Keygem} alt="" />
	</a>
	<a class="vendor-card">
		<p>uk:</p>
		<img src={Prototypist} alt="" />
	</a>
	<a class="vendor-card">
		<p>oce:</p>
		<img src={Keebzncables} alt="" />
	</a>
	<a class="vendor-card">
		<p>sea:</p>
		<img src={Ilumkb} alt="" />
	</a>
	<a class="vendor-card">
		<p>cn:</p>
		<img src={Zfrontier} alt="" />
	</a>
	<a class="vendor-card">
		<p>worldwide:</p>
		<img src={Keyreative} alt="" />
	</a>
</div>

<h1>kitting</h1>
<div class="image-grid">
	<ProjectImage
		imageSource={"https://i.imgur.com/or9PacX.png"}
		{heightOverride}
		headerText={"BASE - $79"}
		headerClass={"astha-smol"}
	></ProjectImage>
	<ProjectImage
		imageSource={"https://i.imgur.com/V2zq62r.png"}
		{heightOverride}
		headerText={"ASTHAN BASE - $79"}
		headerClass={"astha-smol"}
	></ProjectImage>
	<ProjectImage
		imageSource={"https://i.imgur.com/smUEqZi.png"}
		{heightOverride}
		headerText={"SPACEBARS - $79"}
		headerClass={"astha-smol"}
	></ProjectImage>
	<ProjectImage
		imageSource={"https://i.imgur.com/1WR6fF6.png"}
		{heightOverride}
		headerText={"ASTHAN ARTIFACTS - $79"}
		headerClass={"astha-smol"}
	></ProjectImage>
	<ProjectImage
		imageSource={"https://i.imgur.com/T7mztT9.png"}
		{heightOverride}
		headerClass={"astha-smol"}
		headerText={"DESKMAT - $20"}
	></ProjectImage>
	<ProjectImage
		imageSource={"https://i.imgur.com/FiI9fqf.png"}
		{heightOverride}
		headerClass={"astha-smol"}
		headerText={"HIBI METAL CAP - $79"}
	></ProjectImage>
</div>
<h1>renders</h1>
<div class="image-grid">
	<ProjectImage imageSource={"https://i.imgur.com/4UMhtJK.png"} {heightOverride}
	></ProjectImage>
	<ProjectImage imageSource={"https://i.imgur.com/RUaORYu.png"} {heightOverride}
	></ProjectImage>
	<ProjectImage imageSource={"https://i.imgur.com/JRUbIFF.png"} {heightOverride}
	></ProjectImage>
	<ProjectImage imageSource={"https://i.imgur.com/AsovnYx.png"} {heightOverride}
	></ProjectImage>
	<ProjectImage imageSource={"https://i.imgur.com/ZQkcTmh.jpg"} {heightOverride}
	></ProjectImage>
	<ProjectImage imageSource={"https://i.imgur.com/Ohy9AcE.png"} {heightOverride}
	></ProjectImage>
	<ProjectImage imageSource={"https://i.imgur.com/YjKajJb.png"} {heightOverride}
	></ProjectImage>
	<ProjectImage imageSource={"https://i.imgur.com/6v3UZJV.png"} {heightOverride}
	></ProjectImage>
	<ProjectImage imageSource={"https://i.imgur.com/A1Ynx76.jpg"} {heightOverride}
	></ProjectImage>
	<ProjectImage imageSource={"https://i.imgur.com/T701lNh.png"} {heightOverride}
	></ProjectImage>
</div>
<div class="astha">
	<CircleSix height={57}></CircleSix>
	<SeventhLogo height={53}></SeventhLogo>
</div>

<style>
	h1,
	h2,
	h3,
	h4 {
		font-family: "Seventh";
		width: 100%;
		text-align: center;
	}
	.fullpage {
		position: absolute;
		width: 100%;
		height: 100vh;
		top: 0;
		left: 0;
		z-index: 1;
		padding: 20px;
		box-sizing: border-box;
	}
	.fullpage-wrapper {
		height: 100vh;
	}
	.astha {
		margin: 30px auto;
		width: fit-content;
		margin-top: 50px;
        display: flex;
        align-items: center;
        gap: 40px;
	}
</style>
