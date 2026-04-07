<script lang="ts">
    import profile from "$lib/assets/profile.jpg";
</script>

<div
    class="flex-row transition duration-300 sm:bg-shade sm:m-4 p-4 rounded-lg h-20 text-white sm:shadow-lg"
>
    <a href="/about" class="flex items-start text-lg h-full sm:w-full">
        <img src={profile} alt="me lying down" class="rounded-full h-full" />

        <div class="sm:ml-4 flex-col text-[0rem] sm:text-lg">
            <p class="flex font-light">Made by the human</p>
            <p class="flex font-bold -mt-1">David Oriols</p>
        </div>
    </a>
</div>
