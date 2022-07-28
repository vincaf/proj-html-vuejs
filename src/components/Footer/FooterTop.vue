<template>
    <div id="footer_top">
        <div class="container">
            <div class="row justify-content-between py-5">
                <div class="col-4">
                    <div class="title">ABOUT THE BLOG</div>
                    <p class="subtitle">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dicta, eligendi eveniet corrupti explicabo molestias qui id dolorem, corporis quae excepturi laborum quidem. Repellendus impedit quae eos, ex aspernatur omnis repudiandae!</p>
                    <p class="subtitle">Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestias expedita aspernatur nam provident maiores, delectus facilis voluptatum aliquam voluptates, sapiente vero necessitatibus at ratione eos natus modi hic unde minima.</p>
                    <div class="title click">VIEW MORE <i class="fa-solid fa-angle-right"></i></div>
                </div>

                <div class="col-3">
                    <div class="title">RECENT POSTS</div>
                    <div class="d-flex">
                        <img class="click" src="../../assets/images/our-office-4-square.jpg" alt="recent-post-1">
                        <div class="ms-2">
                            <p class="mb-1 click">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                            <p class="subtitle">12:53 AM Dec 19th</p>
                        </div>
                    </div>
                    <div class="d-flex">
                        <img class="click" src="../../assets/images/our-office-5-square.jpg" alt="recent-post-1">
                        <div class="ms-2">
                            <p class="mb-1 click">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                            <p class="subtitle">12:53 AM Dec 19th</p>
                        </div>
                    </div>
                </div>

                <div class="col-3">
                    <div class="title">RECENT COMMENTS</div>
                    <div class="comment">
                        <div>
                            <i class="fa-solid fa-angle-right active"></i><span class="fw-bold ms-1">John Doe</span><span class="ms-1">commented on</span><span class="ms-1 active">lorem ipsum dolor sit amet.</span>
                        </div>
                        <p class="subtitle">12:53 AM Dec 19th</p>
                    </div>

                    <div class="comment">
                        <div>
                            <i class="fa-solid fa-angle-right active"></i><span class="fw-bold ms-1">John Doe</span><span class="ms-1">commented on</span><span class="ms-1 active">lorem ipsum dolor sit amet.</span>
                        </div>
                        <p class="subtitle">12:53 AM Dec 19th</p>
                    </div>
                </div>

                <div class="col-2">
                    <div class="title">CATEGORIES</div>
                    <div class="d-flex flex-wrap">
                        <span class="tags" v-for="(category, index) in categories" :key="index"> {{category}} </span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  data(){
        return{
            categories: [ 'GADGETS', 'PHOTOGRAPHY', 'LIFESTYLE', 'FASHION', 'RECIPES', 'TRAVEL', 'BUSINESS', 'ARCHITECTURE', 'REVIEWS', 'SPORTS', 'VIDEO', 'TECHNOLOGY', 'DESIGN',],
        }
  }
}
</script>

<style lang="scss" scoped>
@import "../../styles/variables.scss";

#footer_top{
    background-color: $bg_footer_top;
    color: $soft_gray;
    font-size: 12px;

    .title{
        font-weight: bold;
        margin-bottom: 20px;
        color: #fff;
    }

    .subtitle{
        font-size: 10px;
        color: $footer_grey;
    }

    img{
        width: 50px;
        height: 50px;
        border-radius: 100%;
        object-fit: cover;
    }

    span{
        &.active{
            color: $blue_primary;
            cursor: pointer;
        }

        &.tags{
            font-size: 9px;
            padding: 2px 6px;
            border-radius: 5px;
            background-color: #000;
            color: #fff;
            font-weight: bold;
            cursor: pointer;
            margin-bottom: 6px;
            margin-right: 7px;
        }
    }

    i{
        &.active{
            color: $blue_primary;
        }
    }

    .click{
        cursor: pointer;
    }
}

</style>