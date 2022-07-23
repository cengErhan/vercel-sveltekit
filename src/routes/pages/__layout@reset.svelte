<script>
import Title from "$lib/title.svelte";
</script>

<main>
    <!-- Content Guides Pages -->
    <div>
        <Title/>
    </div>
    <slot></slot>
</main>

<style>
    main {
        color: darkorange;
        display: flex;
        flex-direction: column;
        text-align: center;
        align-items: center;
        justify-content: center;
    }
</style>

