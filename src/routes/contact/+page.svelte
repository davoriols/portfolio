<script lang="ts">
    import Whitecard from "$lib/components/whitecard.svelte";
    import Matrix from "$lib/components/contactmatrix/matrix.svelte";
</script>

<Whitecard>
    <div class="text-[15rem] font-serif shrink">
        <h1 class="-mt-10">Contact</h1>
    </div>
    <div class="ml-10 mt-10 shrink">
        <p class="text-2xl">Lets build something together!</p>
        <br />
        <p class="text-2xl">
            Feel free to take a look at my resume or contact me in any of these
            platforms:
        </p>
        <Matrix></Matrix>
    </div>
</Whitecard>
