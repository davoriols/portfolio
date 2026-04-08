<script lang="ts">
    import Whitecard from "$lib/components/whitecard.svelte";
    import Matrix from "$lib/components/contactmatrix/matrix.svelte";
</script>

<Whitecard>
    <div
        class="text-[5rem] md:text-[8rem] lg:text-[12rem] xl:text-[15rem] font-serif"
    >
        <h1 class="-mt-10">Contact</h1>
    </div>
    <div class="sm:text-xl xl:text-2xl mx-6 xl:mx-10 mt-10 xl:w-132">
        <p class="">Lets build something together!</p>
        <br />
        <p class="">
            Feel free to take a look at my resume or contact me in any of these
            platforms:
        </p>
    </div>
    <div class="xl:ml-10 xl:mt-10 shrink flex-wrap">
        <Matrix></Matrix>
    </div>
</Whitecard>
