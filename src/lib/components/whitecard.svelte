<script lang="ts">
    import Back from "./back.svelte";

    let { back = true, children } = $props();
</script>

<div
    class="bg-white h-full rounded-xl flex-1 inset-shadow-sm/20 relative overflow-auto"
>
    {#if back}
        <Back></Back>
    {/if}
    <div class="ml-40 mt-20">
        {@render children()}
    </div>
</div>
