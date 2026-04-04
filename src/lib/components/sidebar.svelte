<script lang="ts">
    import Button from "./button.svelte";
    import Avatar from "./avatar.svelte";

    const data = {
        buttons: [
            { name: "home", destination: "/" },
            { name: "about", destination: "/about" },
            { name: "projects", destination: "/projects" },
        ],
    };
</script>

<aside class="flex flex-col w-xs h-screen">
    <div class="m-6 text-white">
        <h1 class="text-4xl">
            <a href="/"> David Oriols </a>
        </h1>
        <p class="font-mono text-lg m-1">V0.0.2</p>
    </div>

    {#each data.buttons as button}
        <Button name={button.name} destination={button.destination}></Button>
    {/each}

    <div class="flex-1"></div>

    <Avatar></Avatar>
</aside>
