<script lang="ts">
    import ARCH from "$lib/assets/tags/ARCH.svg"
    import Cpp from "$lib/assets/tags/C++.svg"
    import CATALAN from "$lib/assets/tags/CATALAN.svg"
    import CLION from "$lib/assets/tags/CLION.svg"
    import CSS from "$lib/assets/tags/CSS.svg"
    import ENGLISH from "$lib/assets/tags/ENGLISH.svg"
    import FRENCH from "$lib/assets/tags/FRENCH.svg"
    import GIT from "$lib/assets/tags/GIT.svg"
    import HTML5 from "$lib/assets/tags/HTML5.svg"
    import JAVASCRIPT from "$lib/assets/tags/JAVASCRIPT.svg"
    import LATEX from "$lib/assets/tags/LATEX.svg"
    import NEOVIM from "$lib/assets/tags/NEOVIM.svg"
    import OBSIDIAN from "$lib/assets/tags/OBSIDIAN.svg"
    import PYTHON from "$lib/assets/tags/PYTHON.svg"
    import SPANISH from "$lib/assets/tags/SPANISH.svg"
    import SVELTE from "$lib/assets/tags/SVELTE.svg"
    import WEBSTORM from "$lib/assets/tags/WEBSTORM.svg"
    import ZEN from "$lib/assets/tags/ZEN.svg"


    const data = {
        languages: [
            {
                src: Cpp,
                alt: "c++ logo",
            },
            {
                src: PYTHON,
                alt: "python logo",
            },
            {
                src: SVELTE,
                alt: "svelte logo",
            },
            {
                src: JAVASCRIPT,
                alt: "javascript logo",
            },
            {
                src: HTML5,
                alt: "html logo",
            },
            {
                src: CSS,
                alt: "css logo",
            },
            {
                src: LATEX,
                alt: "latex logo",
            },
        ],

        tools: [
            {
                src: ZEN,
                alt: "zen logo",
            },
            {
                src: CLION,
                alt: "clion logo",
            },
            {
                src: NEOVIM,
                alt: "neovim logo",
            },
            {
                src: GIT,
                alt: "git logo",
            },
            {
                src: OBSIDIAN,
                alt: "obsidian logo",
            },
            {
                src: WEBSTORM,
                alt: "webstorm logo",
            },
            {
                src: ARCH,
                alt: "arch logo",
            },
        ],
        idiomas: [
            {
                src: ENGLISH,
                alt: "english logo",
            },
            {
                src: FRENCH,
                alt: "french logo",
            },
            {
                src: SPANISH,
                alt: "spanish logo",
            },
            {
                src: CATALAN,
                alt: "catalan logo",
            },
        ],
    };
</script>

<div class="flex flex-col flex-wrap lg:w-full">
    <div>
        <h1 class="text-xl font-bold">Languages I know</h1>
        <div class="flex flex-row flex-wrap m-2">
            {#each data.languages as language}
                <img src={language.src} class="m-1" alt={language.alt} />
            {/each}
        </div>
        <h1 class="text-xl font-bold">Human languages I know</h1>
        <div class="flex flex-row flex-wrap m-2">
            {#each data.idiomas as idioma}
                <img src={idioma.src} class="m-1" alt={idioma.alt} />
            {/each}
        </div>
        <h1 class="text-xl font-bold">Tools I use</h1>
        <div class="flex flex-row flex-wrap m-2">
            {#each data.tools as tool}
                <img src={tool.src} class="m-1" alt={tool.alt} />
            {/each}
        </div>
    </div>
</div>
