<template>
  <section>
    <div class="container">
        <div class="signboard fst-italic">
            Get in Touch
        </div>
    </div>
    <FooterTop />
    <FooterLow />
  </section>
</template>

<script>
import FooterTop from './FooterTop.vue';
import FooterLow from './FooterLow.vue';

export default {
    name: 'MainWeb',
    
    components: {
    FooterTop,
    FooterLow,
  }
}
</script>

<style lang="scss" scoped>
@import "../../styles/variables.scss";

.signboard{
    background-color: $blue_primary;
    color: #fff;
    width: 120px;
    padding: 5px;
    text-align: center;
    font-family:'Times New Roman', Times, serif;
    position: relative;
    top: 20px;
}

</style>