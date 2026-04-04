<script lang="ts">
    import "./layout.css";
    import favicon from "$lib/assets/favicon.svg";
    import Sidebar from "$lib/components/sidebar.svelte";

    let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>

<div class="flex-row flex bg-blue-400">
    <Sidebar />
    {@render children()}
</div>
