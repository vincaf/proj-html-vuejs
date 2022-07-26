<template>
  <section>
    <div class="header_menu d-flex">
        <div class="container">
            <ul class="d-flex list-unstyled mb-0 py-3 align-items-center">
                <li class="slogan">Everything about Lifestyle, Travel and Gadgets!</li>
                <li>SIGN IN</li>
                <li>ABOUT US</li>
                <li>CONTACT US</li>
                <li>BUY NOW</li>
            </ul>
        </div>
    </div>
    <div class="logo py-4">
        <div class="container">
            <img src="../assets/images/logo-default-slim.png" alt="logo">
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

.header_menu{
    background-color: $blue_primary;
    color: #fff;

    ul{
        .slogan{
            opacity: .7;
        }

        li{
            margin-right: 10px;
            font-size: 10px;
            opacity: .9;
        }
    }
}

.logo{
    img{
        width: 7%;
    }
}
</style>