<script lang="ts">
    import Button from "./sidebarbutton.svelte";
    import Avatar from "./avatar.svelte";
    import Contact from "./contact.svelte";

    const data = {
        buttons: [
            { name: "home", destination: "/" },
            { name: "projects", destination: "/projects" },
            { name: "about", destination: "/about" },
        ],
    };
</script>

<aside class="flex flex-col w-xs h-screen">
    <div class="m-6 text-white">
        <h1 class="text-4xl">
            <a href="/"> David Oriols </a>
        </h1>
        <p class="font-mono text-lg m-1">V0.0.3</p>
    </div>

    {#each data.buttons as button}
        <Button name={button.name} destination={button.destination}></Button>
    {/each}

    <div class="flex-1"></div>

    <Contact></Contact>

    <Avatar></Avatar>
</aside>
