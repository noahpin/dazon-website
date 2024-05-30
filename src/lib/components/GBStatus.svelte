<script>
	export let status = "soon";
    export let customStatus = null;
	let statuses = {
		soon: {
			bg: "#b1b1b9",
			color: "black",
			text: "Coming Soon",
		},
		ic: {
			bg: "#80ff00",
			color: "black",
			text: "Interest Check Live",
		},
		gb: {
			bg: "#8c00ff",
			color: "black",
			text: "Group Buy Live",
		},
		post: {
			bg: "white",
			color: "black",
			text: "Group Buy Complete",
		},
	};
</script>

<div
	class="pill"
	style={`color: ${statuses[status].color};background: ${statuses[status].bg};`}
>
	{customStatus || statuses[status].text  }
</div>

<style>
	.pill {
        border-radius: 100px;
        padding: 15px 20px;
        width: fit-content;
        font-weight: bolder !important;
        min-width: 100px;
	}
</style>
