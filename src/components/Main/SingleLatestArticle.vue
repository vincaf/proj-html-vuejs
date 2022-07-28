<template>
    <div class="article">
        <img class="w-100" :src="imgUrl" :alt="title">
        <div class="info d-flex mt-3">
            <div class="date">
                <div class="day text-center">12</div>
                <div class="month text-center">JAN</div>
            </div>
            <div class="text ms-3">
                <h5 class="title fw-bold"> {{ title }} </h5>
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
</template>

<script>
export default {
    props:{
        'title': String,
        'imgUrl': String,
    }
}
</script>

<style lang="scss" scoped>
@import "../../styles/variables.scss";

.article{
    margin-bottom: 60px;

    img{
        cursor: pointer;
    }

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

        .title{
            cursor: pointer;
        }

        p{
            font-size: 13px;
            color: $text_grey;
            cursor: pointer;
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

</style>