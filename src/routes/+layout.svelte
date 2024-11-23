<script lang="ts">
	import "../app.css";
	import Pagina from "../template/Pagina.svelte";
	let { children } = $props();
</script>

<Pagina>
	{@render children()}
</Pagina>
