<script lang="ts">
    import "./layout.css";
    import favicon from "$lib/assets/favicon.svg";
    import Sidebar from "$lib/components/sidebar/sidebar.svelte";

    let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>

<div class="flex-row flex">
    <Sidebar />
    {@render children()}
</div>
