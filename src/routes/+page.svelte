<script>
	import ProjectImage from "$lib/components/ProjectImage.svelte";
	import anim from "$lib/assets/synthesize-anim.mp4"
	import gif from "$lib/assets/synthesize-anim.gif";
</script>

<h2>projects</h2>
<img class="syn" src={gif} />
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
	}
</style>