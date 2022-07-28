<template>
    <div class="social">
        <div id="twitter">
            <div class="title">LATEST FROM TWITTER</div>
            <div class="tweet py-2 d-flex">
                <i class="fa-brands fa-twitter"></i>
                <div class="tweet-detail">
                    <div class="text">
                        <div>If you have any suggestions for the next updates, let us know.</div>
                    </div>
                    <div class="tweet-date">
                        <div>01:05 PM Sep 18th</div>
                    </div>
                </div>
            </div>

            <div class="tweet py-2 d-flex">
                <i class="fa-brands fa-twitter"></i>
                <div class="tweet-detail">
                    <div class="text">
                        <div>We have just updated Porto Admin. Check the changelog for more information.</div>
                    </div>
                    <div class="tweet-date">
                        <div>01:04 PM Sep 18th</div>
                    </div>
                </div>
            </div>
        </div>

        <div id="instagram">
            <div class="title py-2">LATEST FROM INSTAGRAM</div>
            <div class="row row-cols-3 flex-wrap gx-0">
                <img class="col" src="../../assets/images/29739607_2020680068220520_4509928046932787200_n.jpg" alt="article_photo">
                <img class="col" src="../../assets/images/30087804_253872848488989_8792603541668626432_n.jpg" alt="article_photo">
                <img class="col" src="../../assets/images/29415620_196477127626244_3250318472361541632_n.jpg" alt="article_photo">
                <img class="col" src="../../assets/images/30078414_1274410412703843_8290935809419247616_n.jpg" alt="article_photo">
                <img class="col" src="../../assets/images/30077195_2066750973610181_3733150062893596672_n.jpg" alt="article_photo">
                <img class="col" src="../../assets/images/29415304_166583630713703_1032667922171953152_n.jpg" alt="article_photo">
            </div>
        </div>

        <div id="tags">
            <div class="title py-3">TAGS</div>
            <div class="d-flex justify-content-between">
                <span class="tags">DESIGN</span>
                <span class="tags">BRANDS</span>
                <span class="tags">VIDEO</span>
                <span class="tags">BUSINESS</span>
                <span class="tags">TRAVEL</span>
            </div>
        </div>

        <div id="facebook">
            <div class="title mb-2">FIND US ON FACEBOOK</div>
            <span class="link-facebook">Okler Themes</span>
        </div>

    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../../styles/variables.scss";

.social{
    .title{
        font-size: 12px;
        font-weight: bold;
    }

    #twitter{
        .tweet-detail{
            font-size: 12px;
            margin-left: 10px;
            
            .text{
                color: $text_grey;
            }

            .tweet-date{
                color: $blue_primary;
            }
        }
    }

    #tags{
        .tags{
            font-size: 9px;
            padding: 2px 6px;
            border-radius: 20px;
            background-color: $light_black;
            color: #fff;
            font-weight: bold;
            cursor: pointer;
        }
    }

    #facebook{
        margin-top: 70px;

        .link-facebook{
            padding: 5px;
            text-align: center;
            font-size: 12px;
            color: $blue_primary;
            border-left: 3px solid #d6d6d6;
            cursor: pointer;
        }
    }
}
</style>