<script>
    export let description;
    export let image = "";
</script>

<div class="body">
    <div class="description">{description}</div>
    <div class="image">
        <img src={image} alt="description">
    </div>
</div>

<style>
    .body {
        padding: 10px 0;
    }

    .description {
        padding: 10px 0;
    }

    .image img {
        width: 100%;
    }
</style>