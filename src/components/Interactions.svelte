<script>
    import FaRegHeart from 'svelte-icons/fa/FaRegHeart.svelte';
    import FaRegComment from 'svelte-icons/fa/FaRegComment.svelte';
</script>

<div class="container">
    <div class = "icons">
        <FaRegHeart />
    </div>

    <div class = "icons">
        <FaRegComment />
    </div>
</div>

<style>
    .container {
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