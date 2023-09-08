<script>
export let width = "100%", height = "100%"
</script>

<div style={`width: ${width}; height: ${height}`}>
	<slot />
</div>

<style>
div {
	overflow: hidden;
	padding: 25px 15px;
	box-sizing: border-box;
	background-color: var(--foreground);
}
</style>