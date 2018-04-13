<template>
    <article class="recipe">
        <div class="thumbnail" style="background-image: url('https://www.metro.ca/userfiles/image/recipes/pizza-saucisse-piquante-2301.jpg')"></div>
        <h1>Title</h1>
        <p>Some nice preview text</p>
    </article>
</template>

<script>

export default {
}

</script>

<style scoped>

.recipe {
    box-sizing: border-box;
    width: 280px;
    padding: 8px;
    border: 1px solid #ccc;
    box-shadow: 0 2px 2px #aaa;
    margin: 10px;
}

.thumbnail {
    background-position: center;
    background-size: cover;
    width: 100%;
    height: 200px;
}

</style>
