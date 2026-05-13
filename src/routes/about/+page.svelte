<script lang="ts">
    import Whitecard from "$lib/components/whitecard.svelte";
    import Aboutbadges from "./aboutbadges.svelte";
</script>

<Whitecard>
    <div
        class="text-[5rem] md:text-[8rem] lg:text-[12rem] xl:text-[15rem] font-serif"
    >
        <h1 class="-mt-10">About me</h1>
    </div>
    <div class="flex flex-row flex-wrap xl:flex-nowrap mt-10">
        <div class="sm:text-xl xl:text-[1.4rem] flex lg:w-132 mx-6 xl:mx-10">
            <p class="">
                I'm David Oriols. Currently undergoing two bachelors degree's in
                mathematics and computer science.
                <br />
                <br />
                I'm always learning new things, from programming to card magic, to
                even skateboarding from time to time.
            </p>
        </div>
        <div class="ml-10 mr-40">
            <Aboutbadges></Aboutbadges>
        </div>
    </div>
</Whitecard>
