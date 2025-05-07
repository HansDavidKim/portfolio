<script>
    //let { children } = $props();
    import "../app.css";
    import Header from '$lib/components/Header.svelte';
</script>
<Header></Header>
<!--{@render children()}-->

<!--1rem = 16px-->
<div class="bg-gray-900 p-4 text-gray-100 w-full h-screen">
    <slot></slot>
</div>