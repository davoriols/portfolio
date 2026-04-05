<script lang="ts">
    import Matrixbutton from "./matrixbutton.svelte";
    import Linkedin from "./logos/linkedin.svelte";
    import { FileBadge } from "@lucide/svelte";
    import Github from "./logos/github.svelte";
    import { Mail } from "@lucide/svelte";

    let data = {
        buttons: [
            {
                bg: "#4ade80",
                fg: "#ffffff",
                data: "Curriculum",
                icon: FileBadge,
                link: "https://drive.google.com/file/d/1k1iy9KrXyNsUHf16dNXlrdyNsl0LqNMK/view?usp=sharing",
            },
            {
                bg: "#3b82f6",
                fg: "#ffffff",
                data: "LinkedIn",
                icon: Linkedin,
                link: "https://www.linkedin.com/in/david-oriols/",
            },
            {
                bg: "#a855f7",
                fg: "#ffffff",
                data: "GitHub",
                icon: Github,
                link: "https://github.com/davoriols",
            },
            {
                bg: "#4b5563",
                fg: "#ffffff",
                data: "e-mail (alias)",
                icon: Mail,
                link: "mailto:duct-kiln-grinning@duck.com",
            },
        ],
    };
</script>

<div class="m-10 mt-20 flex flex-row">
    {#each data.buttons as button}
        <Matrixbutton props={button}></Matrixbutton>
    {/each}
</div>
