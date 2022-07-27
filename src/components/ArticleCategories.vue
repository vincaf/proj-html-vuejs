<template>
  <section>
    <div class="container">
        <div class="d-flex justify-content-around py-5">
            <span>GADGETS</span>
            <span>PHOTOGRAPHY</span>
            <span>LIFESTYLE</span>
            <span>FASHION</span>
            <span>RECIPES</span>
            <span>TRAVEL</span>
        </div>
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../styles/variables.scss";

section{
    background-color: $blue_darker;

    span{
        background-color: $light_black;
        color: #fff;
        padding: 15px 30px;
        font-size: 10px;
        font-weight: bold;
        width: 150px;
        text-align: center;
    }
}
</style>