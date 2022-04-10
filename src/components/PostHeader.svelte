<script>
    export let avatar;
    export let author;
    export let title;
</script>

<div class="header">
    <div class="avatar">
        <img src={avatar} alt="user-avatar">
    </div>
    <div class="author">{author} - {title}</div>
</div>

<style>
    .header {
        display: flex;
        align-items: center;
        border-bottom: 1px solid black;
        padding: 10px 0;
        font-weight: bold;
    }

    .avatar {
        border-radius: 25px;
        overflow: hidden;
        margin-right: 10px;
    }

    .avatar img {
        width: 50px;
    }

    /* .author {}

    .title {} */
</style>