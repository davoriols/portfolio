<script lang="ts">
    import profile from "$lib/assets/profile.jpg";
</script>

<div
    class="flex-row transition duration-300 bg-shade m-4 p-4 rounded-lg h-20 text-white shadow-lg"
>
    <a href="/about" class="flex items-start text-lg w-full h-full">
        <img src={profile} alt="me lying down" class="rounded-full h-full" />

        <div class="ml-4 flex-col">
            <p class="flex font-light">Made by the human</p>
            <p class="flex text-lg font-bold -mt-1">David Oriols</p>
        </div>
    </a>
</div>
