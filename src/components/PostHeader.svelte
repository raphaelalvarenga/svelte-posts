<script>
    import Avatar from './Avatar.svelte';
    
    export let avatar;
    export let author;
    export let title;
</script>

<div class="header">
    <Avatar src = {avatar} />
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
</style>