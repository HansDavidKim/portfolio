<script>
    let { children } = $props();
    import "../app.css";
    import Header from '$lib/components/Header.svelte';
</script>
<Header></Header>
{@render children()}