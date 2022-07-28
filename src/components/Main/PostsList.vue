<template>
  <section>
    <div class="container">
        <div class="row py-4 justify-content-between">
            <div class="col-3">
                <ul class="list-unstyled">
                    <li class="title mb-2">POPULAR POST</li>

                    <li class="d-flex article">
                        <img class="article_img" src="../../assets/images/blog-55.jpg" alt="pic articolo">
                        <div class="ms-2">
                            <div class="article_title">Simple Ways to Have a Pretty Face</div>
                            <div class="article_date">January 12, 2019</div>
                        </div>
                    </li>

                    <li class="d-flex article">
                        <img class="article_img" src="../../assets/images/blog-55.jpg" alt="pic articolo">
                        <div class="ms-2">
                            <div class="article_title">Simple Ways to Have a Pretty Face</div>
                            <div class="article_date">January 12, 2019</div>
                        </div>
                    </li>
                    
                    <li class="d-flex article">
                        <img class="article_img" src="../../assets/images/blog-55.jpg" alt="pic articolo">
                        <div class="ms-2">
                            <div class="article_title">Simple Ways to Have a Pretty Face</div>
                            <div class="article_date">January 12, 2019</div>
                        </div>
                    </li>

                    <li class="d-flex article">
                        <img class="article_img" src="../../assets/images/blog-55.jpg" alt="pic articolo">
                        <div class="ms-2">
                            <div class="article_title">Simple Ways to Have a Pretty Face</div>
                            <div class="article_date">January 12, 2019</div>
                        </div>
                    </li>

                    <li class="d-flex article">
                        <img class="article_img" src="../../assets/images/blog-55.jpg" alt="pic articolo">
                        <div class="ms-2">
                            <div class="article_title">Simple Ways to Have a Pretty Face</div>
                            <div class="article_date">January 12, 2019</div>
                        </div>
                    </li>

                </ul>
            </div>

            <div class="col-3">
                <ul class="list-unstyled">
                    <li class="title mb-2">RECENT POST</li>

                    <li class="d-flex article">
                        <img class="article_img" src="../../assets/images/blog-55.jpg" alt="pic articolo">
                        <div class="ms-2">
                            <div class="article_title">Simple Ways to Have a Pretty Face</div>
                            <div class="article_date">January 12, 2019</div>
                        </div>
                    </li>

                    <li class="d-flex article">
                        <img class="article_img" src="../../assets/images/blog-55.jpg" alt="pic articolo">
                        <div class="ms-2">
                            <div class="article_title">Simple Ways to Have a Pretty Face</div>
                            <div class="article_date">January 12, 2019</div>
                        </div>
                    </li>
                    
                    <li class="d-flex article">
                        <img class="article_img" src="../../assets/images/blog-55.jpg" alt="pic articolo">
                        <div class="ms-2">
                            <div class="article_title">Simple Ways to Have a Pretty Face</div>
                            <div class="article_date">January 12, 2019</div>
                        </div>
                    </li>

                    <li class="d-flex article">
                        <img class="article_img" src="../../assets/images/blog-55.jpg" alt="pic articolo">
                        <div class="ms-2">
                            <div class="article_title">Simple Ways to Have a Pretty Face</div>
                            <div class="article_date">January 12, 2019</div>
                        </div>
                    </li>

                    <li class="d-flex article">
                        <img class="article_img" src="../../assets/images/blog-55.jpg" alt="pic articolo">
                        <div class="ms-2">
                            <div class="article_title">Simple Ways to Have a Pretty Face</div>
                            <div class="article_date">January 12, 2019</div>
                        </div>
                    </li>

                </ul>
            </div>

            <div class="col-4">
                <ul class="list-unstyled">
                    <li class="title mb-2">FEATURED POST</li>
                    <div class="box d-flex flex-column justify-content-end">
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
export default {

}
</script>

<style lang="scss" scoped>
@import "../../styles/variables.scss";

li{
    &.title{
        font-size: 12px;
        font-weight: bold;
    }

    &.article{
        padding: 10px 0;
        border-bottom: 1px solid #d6d6d6;
    }

    .article_img{
        width: 50px;
        height: 50px;
        object-fit: cover;
    }

    .article_title{
        font-size: 12px;
    }

    .article_date{
        font-size: 10px;
        color: $text_grey;
    }
}

.col-4{
    .box{
        background-image: url("../../assets/images/blog-66.jpg");
        background-size: cover;
        height: 150px;
        width: 375px;
        padding: 20px;
        margin: 30px 0;

        .category{
            font-size: 10px;
            width: 56px;
            padding: 5px;
            font-weight: bold;
            color: #fff;
            background-color: $blue_primary;
        }

        .title{
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