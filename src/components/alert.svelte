<script>
/**
 * 
 * @type{"primary" | "success" | "warning" | "alert" | "natural"}
 * */
export let color = "primary"
</script>


<div class={`alert-c ${color}`}>
	<slot />
</div>

<style>
.alert-c {
	display: block;
	width: 100%;
	--bg-color: var(--primary);
	background: var(--bg-color);
	padding: 15px 20px;
	margin: 10px 0;
	border-radius: 8px;
	box-sizing: border-box;
}

.primary {
	--bg-color: var(--primary);
}

.alert {
	--bg-color: var(--alert);
}

.success {
	--bg-color: var(--success);
}

.warning {
	--bg-color: var(--warning);
}

.natural {
	--bg-color: var(--natural);
}

</style>