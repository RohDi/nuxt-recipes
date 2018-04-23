<template>
  <section class="single-recipe">
      <h1>{{ recipe.title }}</h1>
      <div>
          <img class="recipe-image" :src="recipe.thumbnail" :alt="recipe.title">
      </div>
      <p>{{ recipe.descriptionText }}</p>
  </section>
</template>

<script>
export default {
    asyncData(context){
        return new Promise((resolve, recejt) => {
            setTimeout( () => {
                resolve({
                    recipe: [
                        {
                            id: "1",
                            title: "Delicious Pizza(ajaxed)",
                            previewText: "Awesome Pizza!",
                            descriptionText: "This is really a delicious meal!",
                            thumbnail: "https://bit.ly/2GVYWM2"
                        },
                        {
                            id: "2",
                            title: "Sea Food Salad(ajaxed)",
                            previewText: "Very tasty indeed!",
                            descriptionText: "This is really a delicious meal!",
                            thumbnail: "https://bit.ly/2qtNwou"
                        }
                    ].find(el => el.id === context.params.id)
                })
            }, 1500)
        })
    }
}
</script>


<style scoped>
.single-recipe {
    display: flex;
    flex-flow: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 30px;
}

.recipe-image {
    width: 500px;
    height: 500px;

}
</style>
