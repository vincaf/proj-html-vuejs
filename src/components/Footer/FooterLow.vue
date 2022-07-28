<template>
    <div id="footer_low">
        <div class="container">
            <div class="d-flex py-3 justify-content-between">
                <div class="d-flex align-items-center">
                    <img src="../../assets/images/logo-footer.png" alt="">
                    <div class="ms-5 copyright">© Copyright 2022. All Rights Reserved</div>
                </div>
                <div class="d-flex align-items-center">
                    <div class="fw-bold click">
                        <i class="fa-solid fa-angle-right me-1"></i> FAQ's
                    </div>
                    <div class="ms-3 fw-bold click">
                        <i class="fa-solid fa-angle-right me-1"></i> Sitemap
                    </div>
                    <div class="ms-3 fw-bold click">
                        <i class="fa-solid fa-angle-right me-1"></i> Contact Us
                    </div>
                </div>
            </div>

            <a href="#"><i class="fa-solid fa-angle-up"></i></a>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../../styles/variables.scss";

#footer_low{
    background-color: $bg_footer_low;
    font-size: 10px;
    color: $grey_nav;

    .container{
        position: relative;
    }

    img{
        width: 15%;
        opacity: .5;
    }

    .copyright{
        opacity: .8;
    }

    a{
        background-color: #444;
        color: #fff;
        font-size: 9px;
        padding: 8px 13px;
        position: absolute;
        right: -140px;
        bottom: 0;
    }

    .click{
        cursor: pointer;
    }
}

</style>