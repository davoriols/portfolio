<script lang="ts">
    import Back from "./back.svelte";

    let { back = true, children } = $props();
</script>

<div
    class="bg-white h-full rounded-xl flex-1 inset-shadow-sm/20 relative overflow-y-scroll custom-scroll"
>
    {#if back}
        <Back></Back>
    {/if}
    <div class="ml-40 mt-20">
        {@render children()}
    </div>
</div>

<style>
    /* Modern browsers — Chrome 121+, Edge 121+, Firefox, Safari 18.2+ */
    * {
        scrollbar-width: 8px;
        scrollbar-color: var(--color-shade) #ffffff00;
    }

    /* Legacy WebKit — older Chrome/Edge/Safari, radius, borders & shadows */
    *::-webkit-scrollbar {
        width: 8px;
        height: 10px;
    }

    *::-webkit-scrollbar-track {
        background-color: #ffffff00;
        border-radius: 0px;
        padding: 6px;
    }

    *::-webkit-scrollbar-thumb {
        background-color: var(--color-shade);
        border-radius: 8px;
        min-height: 30px;
    }

    *::-webkit-scrollbar-thumb:hover {
        background-color: #2563eb;
    }

    *::-webkit-scrollbar-thumb:active {
        background-color: #1d4ed8;
    }

    *::-webkit-scrollbar-button {
        display: none;
        width: 0;
        height: 0;
    }
</style>
