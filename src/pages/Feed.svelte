<script>
    import { onMount } from "svelte";
    import Post from "../components/Post.svelte";

    let posts = [];

    onMount(async () => {
        const req = await fetch("http://localhost:5000/posts");
        posts = await req.json();
    })
</script>

{#each posts as post (post.id)}
    <Post {post} />
{/each}