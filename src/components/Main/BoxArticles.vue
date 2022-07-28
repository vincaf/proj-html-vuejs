<template>
    <div class="box d-flex flex-column justify-content-end">
        <img :src="imgUrl" :alt="title">
        <span class="category">
            {{ category }}
        </span>
        <div class="title">
            {{ title }}
        </div>
        <div class="text mt-1">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus repudiandae expedita.
        </div>
    </div>
</template>

<script>

export default {
    props:{
        'category': String,
        'title': String,
        'imgUrl': String,
    }
}
</script>

<style lang="scss" scoped>
@import "../../styles/variables.scss";

.box{
    background-color: #000;
    height: 200px;
    width: 375px;
    padding: 20px;
    margin-bottom: 30px;
    cursor: pointer;
    position: relative;
    &:hover{
        background-color: #fff;

        img{
            border: 5px solid #fff;
            opacity: 1;
        }

        .text{
            display: inline-block;
        }
    }


    img{
        height: 200px;
        width: 375px;
        left: 0;
        top: 0;
        opacity: .7;
        position: absolute;
    }

    .category{
        z-index: 1;
        font-size: 10px;
        width: 90px;
        padding: 5px;
        font-weight: bold;
        text-align: center;
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

    .text{
        display: none;
        font-size: 10px;
        color: $soft_gray;
        z-index: 1;
    }
}
</style>