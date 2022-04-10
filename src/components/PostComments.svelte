<script>
    import FaRegHeart from 'svelte-icons/fa/FaRegHeart.svelte';
    import FaHeart from 'svelte-icons/fa/FaHeart.svelte';
    import FaRegComment from 'svelte-icons/fa/FaRegComment.svelte';

    export let comments = [];
</script>

<div class="comments">
    {#each comments as comment (comment.id)}
        <div class="comment">
            <div class="author">
                <div class="avatar">
                    <img src={comment.avatar} alt="user">
                </div>
                {comment.name}
            </div>

            <div class="description">{comment.comment}</div>

            <div class="likes">
                <div class = "icons">
                    <FaRegHeart />
                </div>

                <div class = "icons">
                    <FaRegComment />
                </div>
            </div>
        </div>
    {/each}
</div>

<style>
    .comments {
        background: rgba(0, 0, 0, 0.1);
        
        border-radius: 8px;
    }

    .comment {
        padding: 20px;
    }

    .author {
        display: flex;
        align-items: center;
        font-weight: bold;
    }

    .avatar {
        width: 50px;
        border-radius: 25px;
        overflow: hidden;
        margin-right: 10px;
    }

    .avatar img {
        width: 50px;
    }

    .description {
        margin-left: 60px;
    }

    .likes {
        margin-top: 15px;
        margin-left: 60px;
        display: flex;
    }

    .icons {
        width: 20px;
    }

    .icons:nth-child(1) {
        margin-right: 10px;
    }
</style>