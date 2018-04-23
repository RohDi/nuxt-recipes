<template>
  <section class="recipes">
      <Recipe
        v-for="recipe in recipes"
        :key="recipe.id"
        :thumbnail="recipe.thumbnail"
        :title="recipe.title"
        :id="recipe.id"
        :previewText="recipe.previewText"
      />
  </section>
</template>

<script>
import Recipe from '@/components/Recipe'

export default {
    components: {
        Recipe
    },
    asyncData(){
        return new Promise((resolve, recejt) => {
            setTimeout( () => {
                resolve({
                    recipes: [
                        {
                            id: "1",
                            title: "Delicious Pizza(ajaxed)",
                            previewText: "Awesome Pizza!",
                            thumbnail: "https://bit.ly/2GVYWM2"
                        },
                        {
                            id: "2",
                            title: "Sea Food Salad(ajaxed)",
                            previewText: "Very tasty indeed!",
                            thumbnail: "https://bit.ly/2qtNwou"
                        }
                    ]
                })
            }, 1500)
        })
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
