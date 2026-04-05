<script lang="ts">
    import { page } from "$app/state";

    let { name, destination } = $props();

    let isActive = $derived(
        page.url.pathname === destination ? "bg-blue-500 shadow-xl" : "",
    );
</script>

<a href={destination} class="flex-row flex">
    <button
        class="flex-1 text-lg transition duration-300 hover:bg-shade mx-4 my-1 rounded-xl h-12 {isActive} text-white pl-4"
    >
        <p class="flex">{name}</p>
    </button>
</a>
