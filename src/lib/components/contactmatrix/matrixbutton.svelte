<script lang="ts">
    let { props } = $props();
    // console.log(props.link);
</script>

<div class="ml-4">
    <a href={props.link} target="_blank">
        <button
            class="custom-btn flex items-center transition duration-300 hover:shadow-xl hover:bg-wshade rounded-2xl h-18 w-55 text-black"
            style="--brand-color: {props.bg}; --fg-color: {props.fg}"
        >
            <!-- <Icon class="flex-1" size="28" /> -->

            <div class="mx-4">
                <props.icon></props.icon>
            </div>

            <p class="text-lg font-extrabold">
                {props.data}
            </p>
        </button>
    </a>
</div>

<style>
    .custom-btn {
        background-color: var(--brand-color);
        color: var(--fg-color);
    }

    .custom-btn:hover {
        filter: brightness(0.9) saturate(1.2);
        transition: 0.3s;
    }
</style>
