<script>
    import FaRegHeart from 'svelte-icons/fa/FaRegHeart.svelte';
    import FaHeart from 'svelte-icons/fa/FaHeart.svelte';
    import FaRegComment from 'svelte-icons/fa/FaRegComment.svelte';
</script>

<div class="comments">
    <div class="comment">
        <div class="author">
            <div class="avatar">
                <img src="https://studiosol-a.akamaihd.net/uploadfile/letras/fotos/2/1/d/0/21d077ea5a8c65c86ef95a9e5b598b69.jpg" alt="user">
            </div>
            Ringo Starr
        </div>

        <div class="description">This is actually a great news! I can't wait to see what is going to happen from that...</div>

        <div class="likes">
            <div class = "icons">
                <FaRegHeart />
            </div>

            <div class = "icons">
                <FaRegComment />
            </div>
        </div>
    </div>
</div>

<style>
    .comments {
        background: rgba(0, 0, 0, 0.1);
        padding: 20px;
        border-radius: 8px;
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