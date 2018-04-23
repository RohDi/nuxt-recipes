<template>
  <section class="recipes">
      <Recipe
        :thumbnail="recipes[0].thumbnail"
        :title="recipes[0].title"
        :id="recipes[0].id"
        :previewText="recipes[0].previewText"
      />
      <Recipe
        :thumbnail="recipes[1].thumbnail"
        :title="recipes[1].title"
        :id="recipes[1].id"
        :previewText="recipes[0].previewText"
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
