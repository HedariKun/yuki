<script>
export let placeholder = ""
</script>

<input placeholder={placeholder} />

<style>
input {
	width: 100%;
	box-sizing: border-box;
	padding: 10px 15px;
	margin: 0;
	background: none;
	border: 0;
	border-bottom: 4px solid var(--foreground);
	color: var(--text);
}

input::placeholder {
	color: var(--text);
	filter: brightness(75%);
}

input:focus {
	border-bottom: 10px solid var(--priamry);
	color:red;
}

</style>