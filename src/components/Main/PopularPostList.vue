<template>
    <li class="d-flex article">
        <img class="article_img" :src="imgUrl" :alt="title">
        <div class="ms-2">
            <div class="article_title"> {{ title }} </div>
            <div class="article_date"> {{ date }} </div>
        </div>
    </li>
</template>

<script>
export default {
    props:{
        'date': String,
        'title': String,
        'imgUrl': String,
    }
}
</script>

<style lang="scss" scoped>
@import "../../styles/variables.scss";

li{

    &.article{
        padding: 10px 0;
        border-bottom: 1px solid #d6d6d6;
        cursor: pointer;
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

</style>