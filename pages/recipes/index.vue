<template>
  <section class="recipes">
      <Recipe
        thumbnail="https://bit.ly/2GVYWM2"
        title="Delicious Pizza"
        previewText="Awesome Pizza"
      />
      <Recipe
          thumbnail="https://bit.ly/2qtNwou"
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
