<script>
	import ProjectImage from "$lib/components/ProjectImage.svelte";
	import anim from "$lib/assets/synthesize-anim.mp4"
	import gif from "$lib/assets/synw.gif";
</script>

<h2>projects</h2>
<div class="syn-w">
<img class="syn" src={gif} />
</div>
<a href="./kam-astha">
	<ProjectImage
		imageSource={"https://i.imgur.com/Xgtnxdd.jpeg"}
		headerClass={"astha-header"}
		headerText={"KAM ASTHA"}
        status={"ic"}
        customStatus={"Group Buy May 31st"}
        forceView={true}
	></ProjectImage></a
>
<br>
<h2>coming soon</h2>
<div class="image-grid">
	<ProjectImage
		imageSource={"https://i.imgur.com/occonX1.png"}
		headerText={"R**W***"}
        status={"soon"}
        heightOverride={"min(300px, 65vh)"}
	></ProjectImage>
	<ProjectImage
		imageSource={"https://i.imgur.com/mDUG8OU.png"}
		headerText={"S*********"}
        status={"soon"}
        heightOverride={"min(300px, 65vh)"}
	></ProjectImage>
</div>

<style>
	.syn {
		width: 100%;
		height: auto;
		margin: 0 auto;
		display: block;
		padding: 50px;
		box-sizing: border-box;
		position: relative;
	}
	.syn-w {
		position: relative
	}
	.syn-w::after {
		content: "";
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		z-index: 1;
		background-color: #fe5000;
		mix-blend-mode: multiply;
	}
</style>