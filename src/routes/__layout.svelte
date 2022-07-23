<script>
import Title from "$lib/title.svelte";
</script>

<header>
    <Title />
</header>

<main>
    <!-- Content Page -->
    <slot></slot>
</main>

<footer>
    <main>
        <div>
            <h1>Footer Block</h1>
        </div>
    </main>
</footer>

<style>
    main {
        display: flex;
        align-items: center;
        text-align: center;
        justify-content: center;
        color: rebeccapurple;
    }
    header {
        color: rebeccapurple;
    }
</style>

