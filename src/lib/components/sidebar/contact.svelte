<script lang="ts">
    import { Send } from "@lucide/svelte";
</script>

<div class="flex-row">
    <button
        class="sm:w-38 transition duration-300 bg-white mx-4 rounded-full h-12 text-shade on hover:bg-wshade"
    >
        <a href="/contact" class="flex text-lg justify-center">
            <div
                class="sm:w-0 sm:h-0 sm:invisible sm:m-0 w-fit h-fit visible m-3"
            >
                <Send></Send>
            </div>
            <p class="text-[0rem] sm:text-lg">Lets connect!</p>
        </a>
    </button>
</div>
