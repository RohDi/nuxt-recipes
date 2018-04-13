<template>
  <section class="recipes">
      <Recipe/>
      <article class="recipe">
          <div class="thumbnail" style="background-image: url('http://cdn0.wideopeneats.com/wp-content/uploads/2016/12/days-order-seafood-restaurant.png')"></div>
          <h1>Title</h1>
          <p>Some nice preview text</p>
      </article>
  </section>
</template>

<script>
import Recipe from '@/components/Recipe'

export default {
    components: {
        Recipe
    }
}
</script>

<style scoped>

.recipes {
    display: flex;
    flex-flow: row wrap;
    justify-content: center;
    align-items: center;
}

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
