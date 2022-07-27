<template>
  <section>
    <div class="header_menu d-flex">
        <div class="container">
            <ul class="d-flex list-unstyled mb-0 py-3">
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
    <hr class="m-0">
    <div class="nav">
        <div class="container">
            <div class="d-flex justify-content-between">
                <div>
                    <ul class="d-flex list-unstyled mb-0 py-3">
                        <li class="active">HOME</li>
                        <li>ELEMENTS</li>
                        <li>FEATURES</li>
                        <li>PAGES</li>
                        <li>PORTFOLIO</li>
                        <li>BLOG</li>
                        <li>SHOP</li>
                    </ul>
                </div>
                <div>
                    <i class="fa-solid fa-magnifying-glass py-3"></i>
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
@import "../styles/variables.scss";

.header_menu{
    background-color: $blue_primary;
    color: #fff;

    ul{
        li{
            margin-right: 10px;
            font-size: 10px;
            opacity: .9;

            &.slogan{
                opacity: .7;
            }
        }
    }
}

.logo{
    img{
        width: 7%;
    }
}

hr{
    opacity: .1;
}

.nav{
    color: $grey_nav;

    ul{
        li{
            margin-right: 30px;
            font-size: 13px;
            font-weight: bold;

            &.active{
                color: $blue_primary;
            }
        }
    }
}
</style>