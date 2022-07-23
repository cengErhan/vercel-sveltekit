<script context="module">
    export async function load({fetch}){
        const res = await fetch('https://jsonplaceholder.typicode.com/posts')
        const guides = await res.json()
        if(res.ok){
            return{
                props: {
                    guides
                }
            }
        }

        return {
            status: res.status,
            error: new Error('Could not fetch the guides')
        }
    }
</script>

<script>
    export let guides
</script>

<main>
    <div class="guides">
        <ul>
            {#each guides as guide}
                <li>
                    <a sveltekit:prefetch href="/pages/post/{guide.id}">{guide.id} {guide.title}</a>
                </li>
            {/each}
        </ul>
    </div>
</main>

<style>
    a{
        text-decoration: none;
        font-size: large;
        color: darkorange;
    }
    main li{
        list-style-type: none;
        padding-top: 20px;
    }
</style>