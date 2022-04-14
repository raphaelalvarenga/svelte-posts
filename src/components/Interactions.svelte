<script>
    import FaRegHeart from 'svelte-icons/fa/FaRegHeart.svelte';
    import FaRegComment from 'svelte-icons/fa/FaRegComment.svelte';

    export let type;
</script>

<div class={`${type === "posts" ? "container-posts" : "container-comments"}`}>
    <div class = {`${type === "posts" ? "icons-post" : "icons-comments"}`}>
        <FaRegHeart />
    </div>

    <div class = {`${type === "posts" ? "icons-post" : "icons-comments"}`}>
        <FaRegComment />
    </div>
</div>

<style>
    .container-posts {
        padding: 30px 0;
        display: flex;
    }

    .container-comments {
        margin-top: 15px;
        margin-left: 60px;
        display: flex;
    }

    .icons-post {
        width: 30px;
    }

    .icons-comments {
        width: 20px;
    }

    .icons-comments:nth-child(1), .icons-post:nth-child(1) {
        margin-right: 10px;
    }
</style>