<script>
    import PostHeader from './PostHeader.svelte';
    import PostBody from './PostBody.svelte';
    import PostLikes from './PostLikes.svelte';
    import PostComments from './PostComments.svelte';
    import PostAddComment from './PostAddComment.svelte';

    export let post;
</script>

<div class="post">
    <PostHeader
        avatar = {post.author.avatar}
        author = {post.author.name}
        title = {post.title}
    />
    <PostBody description = {post.description} image = {post.imageUrl} />
    <PostLikes />
    <PostComments comments = {post.comments} />
    <PostAddComment />
</div>

<style>
    .post {
        max-width: 800px;
        width: 100%;
        margin: auto;
        padding: 20px;
        box-shadow: 5px 5px 15px rgb(150, 150, 150);
        border-radius: 8px;
        margin-bottom: 50px;
    }
</style>