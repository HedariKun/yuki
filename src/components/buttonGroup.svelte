<script>
export let space = "100px"

/**
 * @type{"row" | "column"}
 * */
export let direction = "row"
</script>

<main style={`gap: ${space}; flex-direction: ${direction};`}>
	<slot />
</main>

<style>
main {
	display: flex;
	flex-wrap: nowrap;
}


</style>