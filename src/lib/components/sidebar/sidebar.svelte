<script lang="ts">
    import Button from "./sidebarbutton.svelte";
    import Avatar from "./avatar.svelte";
    import Contact from "./contact.svelte";
    import { House, ChefHat, User } from "@lucide/svelte";

    const data = {
        buttons: [
            { name: "Home", destination: "/", icon: House },
            { name: "Projects", destination: "/projects", icon: ChefHat },
            { name: "About", destination: "/about", icon: User },
        ],
    };
</script>

<aside class="flex flex-col w-fit sm:w-xs shrink-0 h-screen">
    <div class="m-6 text-white">
        <h1 class="text-4xl sm:text-[0px] font-sans -mb-2 font-extrabold">
            <a href="/"> D</a>
        </h1>
        <h1 class="text-[0rem] sm:text-4xl font-sans -mb-2 font-extrabold">
            <a href="/"> David Oriols </a>
        </h1>
        <p class="font-mono text-[0rem] sm:text-lg m-1">V0.1.0</p>
    </div>

    {#each data.buttons as button}
        <Button
            name={button.name}
            destination={button.destination}
            Icon={button.icon}
        ></Button>
    {/each}

    <div class="flex-1"></div>

    <Contact></Contact>

    <Avatar></Avatar>
</aside>
