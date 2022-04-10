<script>
    import FaRegHeart from 'svelte-icons/fa/FaRegHeart.svelte';
    import FaHeart from 'svelte-icons/fa/FaHeart.svelte';
    import FaRegComment from 'svelte-icons/fa/FaRegComment.svelte';
</script>

<div class="likes">
    <div class = "icons">
        <FaRegHeart />
    </div>

    <div class = "icons">
        <FaRegComment />
    </div>
</div>

<style>
    .likes {
        padding: 30px 0;
        display: flex;
    }

    .icons {
        width: 30px;
    }

    .icons:nth-child(1) {
        margin-right: 10px;
    }
</style>