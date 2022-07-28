<template>
  <section>
    <div class="container">
        <div class="d-flex flex-wrap justify-content-between pt-5 pb-3">
            <div class="box d-flex flex-column justify-content-end">
                <span class="category">
                    PHOTOGRAPHY
                </span>
                <div class="title">
                    How To Take Better Concert Pictures in 30 Seconds
                </div>
            </div>

            <div class="box d-flex flex-column justify-content-end">
                <span class="category">
                    PHOTOGRAPHY
                </span>
                <div class="title">
                    How To Take Better Concert Pictures in 30 Seconds
                </div>
            </div>

            <div class="box d-flex flex-column justify-content-end">
                <span class="category">
                    PHOTOGRAPHY
                </span>
                <div class="title">
                    How To Take Better Concert Pictures in 30 Seconds
                </div>
            </div>

                        <div class="box d-flex flex-column justify-content-end">
                <span class="category">
                    PHOTOGRAPHY
                </span>
                <div class="title">
                    How To Take Better Concert Pictures in 30 Seconds
                </div>
            </div>

            <div class="box d-flex flex-column justify-content-end">
                <span class="category">
                    PHOTOGRAPHY
                </span>
                <div class="title">
                    How To Take Better Concert Pictures in 30 Seconds
                </div>
            </div>

            <div class="box d-flex flex-column justify-content-end">
                <span class="category">
                    PHOTOGRAPHY
                </span>
                <div class="title">
                    How To Take Better Concert Pictures in 30 Seconds
                </div>
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

section{
    background-color: $bg_light_grey;

    .box{
        background-image: url("../../assets/images/blog-46.jpg");
        background-size: cover;
        height: 200px;
        width: 375px;
        padding: 20px;
        margin-bottom: 30px;

        .category{
            font-size: 10px;
            width: 90px;
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
}
</style>