<script lang="ts">
    const data = {
        languages: [
            {
                src: "./src/lib/assets/tags/C++.svg",
                alt: "c++ logo",
            },
            {
                src: "./src/lib/assets/tags/PYTHON.svg",
                alt: "python logo",
            },
            {
                src: "./src/lib/assets/tags/SVELTE.svg",
                alt: "svelte logo",
            },
            {
                src: "./src/lib/assets/tags/JAVASCRIPT.svg",
                alt: "javascript logo",
            },
            {
                src: "./src/lib/assets/tags/HTML5.svg",
                alt: "html logo",
            },
            {
                src: "./src/lib/assets/tags/CSS.svg",
                alt: "css logo",
            },
            {
                src: "./src/lib/assets/tags/LATEX.svg",
                alt: "latex logo",
            },
        ],

        tools: [
            {
                src: "./src/lib/assets/tags/ZEN.svg",
                alt: "zen logo",
            },
            {
                src: "./src/lib/assets/tags/CLION.svg",
                alt: "clion logo",
            },
            {
                src: "./src/lib/assets/tags/NEOVIM.svg",
                alt: "neovim logo",
            },
            {
                src: "./src/lib/assets/tags/GIT.svg",
                alt: "git logo",
            },
            {
                src: "./src/lib/assets/tags/OBSIDIAN.svg",
                alt: "obsidian logo",
            },
            {
                src: "./src/lib/assets/tags/WEBSTORM.svg",
                alt: "webstorm logo",
            },
            {
                src: "./src/lib/assets/tags/ARCH.svg",
                alt: "arch logo",
            },
        ],
        idiomas: [
            {
                src: "./src/lib/assets/tags/ENGLISH.svg",
                alt: "english logo",
            },
            {
                src: "./src/lib/assets/tags/FRENCH.svg",
                alt: "french logo",
            },
            {
                src: "./src/lib/assets/tags/SPANISH.svg",
                alt: "spanish logo",
            },
            {
                src: "./src/lib/assets/tags/CATALAN.svg",
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
