<script>
    import Title from "$lib/title.svelte";
</script>

<main>
    <Title />
    <slot></slot>
</main>

<style>
    main {
        color: olive;
    }
</style>