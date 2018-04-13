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

</style>
