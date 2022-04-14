<script>
    import MdSend from 'svelte-icons/md/MdSend.svelte';
</script>

<div style = "display: flex; align-items: center; margin-top: 30px;">
    <div><input type="text" placeholder="Type something..."></div>
    <div class="send-container"><MdSend /></div>
</div>

<style>
    input {
        margin-right: 10px;
        border: 2px solid rgba(0, 0, 0, 0.5);
        border-radius: 20px;
        height: 30px;
        padding-left: 10px;
    }

    .send-container {
        width: 30px;
        transform: rotateZ(-20deg);
        margin-top: -10px;
    }
</style>