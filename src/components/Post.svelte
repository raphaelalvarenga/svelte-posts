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
        max-width: 800px;
        width: 100%;
        margin: auto;
        padding: 20px;
        box-shadow: 5px 5px 15px black;
        border-radius: 8px;
    }
</style>