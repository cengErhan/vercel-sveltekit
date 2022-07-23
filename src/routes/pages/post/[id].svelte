<script context="module">
    export async function load({ fetch, params}){
        const id = params.id
        const res = await fetch(`https://jsonplaceholder.typicode.com/posts/${id}`)
        const guide = await res.json()
        if(res.ok){
            return{
                props: {
                    guide, id
                }
            }
        }

        return {
            status: 301,
            //error: new Error('Could not fetch the guides')
            redirect: '/pages'
        }
    }
</script>

<script>
    export let guide, id
</script>

<div class="guide">
    <h2>{guide.title}</h2>
    <p>{guide.body}</p>
    <p>{id}</p>
</div>

<style>
    .guide {
        margin-top: 40px;
        padding: 10px;
        border: 1px dotted olive;
        color: olive;
        align-items: center;
        text-align: center;
        justify-content: end;
    }
</style>

