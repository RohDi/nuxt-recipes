<template>
  <section class="recipes">
      <Recipe
        thumbnail="https://www.metro.ca/userfiles/image/recipes/pizza-saucisse-piquante-2301.jpg"
        title="Delicious Pizza"
        previewText="Awesome Pizza"
      />
      <Recipe
          thumbnail="http://cdn0.wideopeneats.com/wp-content/uploads/2016/12/days-order-seafood-restaurant.png"
          title="Sea Food Salad"
          previewText="Very tasty indeed!"
       />
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
