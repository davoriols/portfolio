<script lang="ts">
    import "./layout.css";
    import favicon from "$lib/assets/favicon.svg";
    import Sidebar from "$lib/components/sidebar/sidebar.svelte";

    let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>

<div class="flex-row flex overflow-hidden h-screen">
    <Sidebar />
    <div class="pt-3 pr-3 pb-3 flex w-full">
        {@render children()}
    </div>
</div>
