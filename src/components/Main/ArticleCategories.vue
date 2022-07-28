<template>
  <section>
    <div class="container">
        <div class="d-flex justify-content-between blue-bar">
          <i class="fa-solid fa-angle-left"></i>
          <span class="my-5 d-flex align-items-center justify-content-center" v-for="(category, index) in categories" :key="index"> {{category}} </span>
          <i class="fa-solid fa-angle-right"></i>
        </div>
    </div>
  </section>
</template>

<script>
export default {
  data(){
        return{
            categories: [ 'GADGETS', 'PHOTOGRAPHY', 'LIFESTYLE', 'FASHION', 'RECIPES', 'TRAVEL'],
        }
  }

}
</script>

<style lang="scss" scoped>
@import "../../styles/variables.scss";

section{
    background-color: $blue_darker;

    .blue-bar{
      height: 140px;
    }

    span{
      background-color: $light_black;
      color: #fff;
      padding: 0 30px;
      font-size: 10px;
      font-weight: bold;
      width: 150px;
      cursor: pointer;

      &:hover{
        border: 5px solid $blue_primary;
      }
    }

    i{
      margin: auto 0;
      cursor: pointer;

      &:hover{
        color: #fff;
      }
    }
}
</style>