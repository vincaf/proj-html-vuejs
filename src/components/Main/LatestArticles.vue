<template>
  <section>
    <div class="container">
        <div class="row py-5">
            <div class="col-9">
                <SingleLatestArticle v-for="article in articles" :key="article.id"
                :title="article.title"
                :imgUrl="article.img" />

                <div class="article-bonus">
                    <div class="row row-cols-3 flex-wrap gx-0">
                        <img class="col" src="../../assets/images/blog-13.jpg" alt="article_photo">
                        <img class="col" src="../../assets/images/blog-16.jpg" alt="article_photo">
                        <img class="col" src="../../assets/images/blog-20.jpg" alt="article_photo">
                        <img class="col" src="../../assets/images/blog-23.jpg" alt="article_photo">
                        <img class="col" src="../../assets/images/blog-29.jpg" alt="article_photo">
                        <img class="col" src="../../assets/images/blog-40.jpg" alt="article_photo">
                    </div>
                    <div class="info d-flex mt-3">
                        <div class="date">
                            <div class="day text-center">12</div>
                            <div class="month text-center">JAN</div>
                        </div>
                        <div class="text ms-3">
                            <h5 class="title fw-bold">How to Make Friends as a Grown-Up</h5>
                            <p class="mt-1">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ad cupiditate nam harum, dolorem quaerat eum dolores quis culpa libero. Ad ipsam ut veniam quod non quidem aliquid nihil, suscipit nulla. [...]</p>
                            <div class="details d-flex justify-content-between">
                                <div>
                                    <span class="icon"><i class="fa-regular fa-user"></i> By</span>
                                    <span class="detail">John Doe</span>
                                    <span class="icon"><i class="fa-regular fa-folder"></i></span>
                                    <span class="detail">Lifestyle, Travel</span>
                                    <span class="icon"><i class="fa-regular fa-comments"></i></span>
                                    <span class="detail">12 Comments</span>
                                </div>
                                <div>
                                    <button>READ MORE</button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="pages d-flex justify-content-end">
                    <div class="text-center"><i class="fa-solid fa-angle-left"></i></div>
                    <div class="text-center active">1</div>
                    <div class="text-center">2</div>
                    <div class="text-center">3</div>
                    <div class="text-center"><i class="fa-solid fa-angle-right"></i></div>
                </div>

            </div>
            <div class="col-3">
                <SocialPost />
            </div>
        </div>
    </div>
  </section>
</template>

<script>
import SingleLatestArticle from './SingleLatestArticle.vue';
import SocialPost from './SocialPost.vue';

export default {
    name: 'LatestArticles',

    components: {
    SingleLatestArticle,
    SocialPost,
    },

    data(){
        return{
            articles: [
                {
                    id: 1,
                    title: "How To Make Friends as a Grown Up",
                    img: require("@/assets/images/blog-54.jpg"),
                },

                {
                    id: 2,
                    title: "Simple Ways to Have a Pretty face",
                    img: require("@/assets/images/blog-55 (1).jpg"),
                },

                {
                    id: 3,
                    title: "Ranking the greatest players in basketball",
                    img: require("@/assets/images/blog-56 (1).jpg"),
                },

                {
                    id: 4,
                    title: "Top Camper Trailer Towing Tips",
                    img: require("@/assets/images/blog-58 (1).jpg"),
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../styles/variables.scss";

.article-bonus{
    margin-bottom: 60px;

    .date{
        .day{
            padding: 5px 0;
            background-color: $bg_light_grey;
            font-size: 12px;
            font-weight: bold;
        }

        .month{
            padding: 2px 5px;
            font-size: 8px;
            background-color: $light_black;
            color: #fff
        }
    }

    .text{

        p{
            font-size: 13px;
            color: $text_grey;
        }

        .details{
            font-size: 12px;

            span{
                margin-right: 5px;

                &.detail{
                    color: $blue_primary;
                    cursor: pointer;
                }
            }

            button{
                font-size: 9px;
                color: $text_grey;
                border: 1px solid $text_grey;
                background-color: #fff;
            }
        }
    }
}

.pages{
    div{
        padding: 5px 8px;
        font-size: 10px;
        border: 1px solid $soft_gray;
        color: $blue_primary;
        cursor: pointer;

        &.active{
            background-color: $blue_primary;
            color: #fff;
        }
    }
}
</style>