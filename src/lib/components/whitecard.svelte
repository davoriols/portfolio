<script lang="ts">
    import Back from "./back.svelte";

    let { back = true, children } = $props();
</script>

<div
    class="mt-3 mb-3 mr-3 bg-white rounded-xl flex-1 inset-shadow-sm/20 relative"
>
    {#if back}
        <Back></Back>
    {/if}
    <div class="ml-40 mt-20">
        {@render children()}
    </div>
</div>
