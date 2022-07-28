<template>
  <section>
    <div class="container">
        <div class="d-flex flex-wrap justify-content-between pt-5 pb-3">
            <BoxArticles v-for="article in articles" :key="article.id"
            :category="article.category"
            :title="article.title"
            :imgUrl="article.img" />
        </div>
    </div>
  </section>
</template>

<script>
import BoxArticles from './BoxArticles.vue';

export default {
    name: 'FeaturedArticles',

    components: {
    BoxArticles,
    },

    data(){
        return{
            articles: [
                {
                    id: 1,
                    category: "PHOTOGRAPHY",
                    title: "How To Take Better Concert Pictures in 30 Seconds",
                    img: require("@/assets/images/blog-46.jpg"),
                },

                {
                    id: 2,
                    category: "GADGETS",
                    title: "Gadgets That Make Your Smarphone Even Smarter",
                    img: require("@/assets/images/blog-47.jpg"),
                },

                {
                    id: 3,
                    category: "TRAVEL",
                    title: "20 Top-Rated Tourist Attractions in Manhattan",
                    img: require("@/assets/images/blog-48.jpg"),
                },

                {
                    id: 4,
                    category: "LIFESTYLE",
                    title: "The Best Way to Ride a Motorcycle",
                    img: require("@/assets/images/blog-49.jpg"),
                },

                {
                    id: 5,
                    category: "TRAVEL",
                    title: "5 Fun Things to Do at the Beach",
                    img: require("@/assets/images/blog-50.jpg"),
                },

                {
                    id: 6,
                    category: "RECIPES",
                    title: "Amazingly Fresh Fruit And Herb Drinks For Summer",
                    img: require("@/assets/images/blog-51.jpg"),
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../styles/variables.scss";

section{
    background-color: $bg_light_grey;
}
</style>