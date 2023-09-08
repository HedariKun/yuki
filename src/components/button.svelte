<script>
export let disabled = false

/**
 * 
 * @type{"plain" | "outline"}
 * */
export let type = "plain"

/**
 * 
 * @type{"primary" | "success" | "warning" | "alert" | "natural"}
 * */
export let color = "primary"
</script>

<button on:click class={`${type} ${color}`}><slot/></button>

<style>
button {
	width: 100%;
	height: 30px;
	font-size: 16px;
	border: none;
	transition: 0.3s;
	border-radius: 8px;
	--button-primary-color: var(--primary);
}

button:hover {
	cursor: pointer;
}

.primary {
	--button-primary-color: var(--primary);
}

.alert {
	--button-primary-color: var(--alert);
}

.success {
	--button-primary-color: var(--success);
}

.warning {
	--button-primary-color: var(--warning);
}

.natural {
	--button-primary-color: var(--natural);
}

.plain {
	background: var(--button-primary-color);
}

.plain:hover {
	filter: brightness(85%);
}

.outline {
	background: rgba(0, 0, 0, 0);
	border: 1px solid var(--button-primary-color);
	color: var(--button-primary-color);
}

.outline:hover {
	background-color: var(--button-primary-color);
	color: var(--text-color);
}

</style>