<script lang="ts">
    import { page } from "$app/state";

    let { name, destination, Icon } = $props();

    let isActive = $derived(
        page.url.pathname === destination ? "bg-blue-500 shadow-xl" : "",
    );
</script>

<a href={destination} class="flex-row flex">
    <button
        class="flex-1 items-center flex-row flex text-lg transition duration-300 hover:bg-shade mx-4 my-1 rounded-xl h-12 {isActive} text-white pl-3"
    >
        <div class="flex">
            <Icon size="25" />
        </div>
        <p class="flex pl-3">{name}</p>
    </button>
</a>
