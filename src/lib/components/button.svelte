<script lang="ts">
    import { page } from "$app/state";

    let { name, destination } = $props();

    let isActive = $derived(
        page.url.pathname === destination ? "bg-blue-500 shadow-xl" : "",
    );
</script>

<button
    class="flex-row transition duration-300 hover:bg-blue-500 mx-4 my-1 rounded-lg h-12 {isActive} text-white pl-4"
>
    <a href={destination} class="flex text-lg">
        {name}
    </a>
</button>
