<script>
    import PostHeader from './PostHeader.svelte';
    import PostBody from './PostBody.svelte';
    import PostLikes from './PostLikes.svelte';
    import PostComments from './PostComments.svelte';
</script>

<div class="post">
    <PostHeader />
    <PostBody />
    <PostLikes />
    <PostComments />
</div>

<style>
    .post {
        border: 2px solid black;
        max-width: 800px;
        width: 100%;
        margin: auto;
        padding: 10px;
    }
</style>