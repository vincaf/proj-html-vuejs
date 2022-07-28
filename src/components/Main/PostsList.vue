<template>
  <section>
    <div class="container">
        <div class="row py-4 justify-content-between">
            <div class="col-3">
                <ul class="list-unstyled">
                    <li class="title mb-2">POPULAR POST</li>
                    <PopularPostList v-for="popularArticle in popularArticles" :key="popularArticle.id" 
                    :date="popularArticle.date"
                    :title="popularArticle.title"
                    :imgUrl="popularArticle.img" />
                </ul>
            </div>

            <div class="col-3">
                <ul class="list-unstyled">
                    <li class="title mb-2">RECENT POST</li>
                    <RecentPostList v-for="recentArticle in recentArticles" :key="recentArticle.id" 
                    :date="recentArticle.date"
                    :title="recentArticle.title"
                    :imgUrl="recentArticle.img" />
                </ul>
            </div>

            <div class="col-4">
                <ul class="list-unstyled">
                    <li class="title mb-2">FEATURED POST</li>
                    <div class="box d-flex flex-column justify-content-end">
                        <img src="../../assets/images/blog-66.jpg" alt="featured_post">
                        <span class="category">
                            RECIPES
                        </span>
                        <div class="title">
                            Tips to Help You Quickly Prepare your Lunch
                        </div>
                    </div>
                    <li class="title mb-2">FEATURED AUTHOR</li>
                    <li class="d-flex align-items-center">
                        <img class="author_img" src="../../assets/images/avatar.jpg" alt="author">
                        <div class="ms-2">
                            <div class="author_title">John Doe</div>
                            <div class="author_text">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Culpa doloremque assumenda veritatis quaerat. Illum minima accusantium</div>
                        </div>
                    </li>
                </ul>
            </div>

        </div>
    </div>
  </section>
</template>

<script>
import PopularPostList from './PopularPostList.vue';
import RecentPostList from './RecentPostList.vue';

export default {
    name: 'PostsList',
    components: {
        PopularPostList,
        RecentPostList,
    },

    data(){
        return{
            popularArticles: [
                {
                    id: 1,
                    date: "January 12, 2019",
                    title: "Simple Ways to Have a Pretty Face",
                    img: require("@/assets/images/blog-55.jpg"),
                },

                {
                    id: 2,
                    date: "January 12, 2019",
                    title: "Ranking the greatest players in basketball",
                    img: require("@/assets/images/blog-56.jpg"),
                },

                {
                    id: 3,
                    date: "January 12, 2019",
                    title: "4 Ways to Look Cool in Glasses",
                    img: require("@/assets/images/blog-57.jpg"),
                },

                {
                    id: 4,
                    date: "January 12, 2019",
                    title: "Top Camper Trailer Towing Tips",
                    img: require("@/assets/images/blog-58.jpg"),
                },

                {
                    id: 5,
                    date: "January 12, 2019",
                    title: "5 Lovely Walks in New York",
                    img: require("@/assets/images/blog-59.jpg"),
                },
            ],

            recentArticles: [
                {
                    id: 1,
                    date: "January 12, 2019",
                    title: "Main Reasons To Stop Texting And Driving",
                    img: require("@/assets/images/blog-65.jpg"),
                },

                {
                    id: 2,
                    date: "January 12, 2019",
                    title: "Tips to Help You Quickly Prepare your Lunch",
                    img: require("@/assets/images/blog-66 (1).jpg"),
                },

                {
                    id: 3,
                    date: "January 12, 2019",
                    title: "Why should I buy a smartwatch?",
                    img: require("@/assets/images/blog-67.jpg"),
                },

                {
                    id: 4,
                    date: "January 12, 2019",
                    title: "The best augmented reality smartglasses",
                    img: require("@/assets/images/blog-68.jpg"),
                },

                {
                    id: 5,
                    date: "January 12, 2019",
                    title: "12 Healthiest Foods to Eat for Breakfast",
                    img: require("@/assets/images/blog-69.jpg"),
                },
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
@import "../../styles/variables.scss";

li{
    &.title{
        font-size: 12px;
        font-weight: bold;
    }
}

.col-4{
    .box{
        background-color: #000;
        height: 150px;
        width: 375px;
        padding: 20px;
        margin: 30px 0;
        cursor: pointer;
        position: relative;

        img{
            height: 150px;
            width: 375px;
            left: 0;
            top: 0;
            opacity: .7;
            position: absolute;
        }

        .category{
            z-index: 1;
            font-size: 10px;
            width: 56px;
            padding: 5px;
            font-weight: bold;
            color: #fff;
            background-color: $blue_primary;
        }

        .title{
            z-index: 1;
            color: #fff;
            font-weight: bold;
            line-height: 18px;
            margin-top: 8px;
        }
    }

    .author_img{
        width: 100px;
        height: 100px;
        object-fit: cover;
    }

    .author_title{
        font-size: 15px;
        font-weight: bold;
        margin-bottom: 5px;
    }

    .author_text{
        font-size: 12px;
        color: $text_grey;
    }
}

</style>