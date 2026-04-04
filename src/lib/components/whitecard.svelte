<script lang="ts">
    let { children } = $props();
</script>

<div class="mt-3 mb-3 mr-3 bg-white rounded-xl flex-1 inset-shadow-sm/20">
    {@render children()}
</div>
