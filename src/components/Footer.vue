<script>
export default {
    name: "Footer"
}
</script>

<template>
    <!-- STORE -->
    <section id="store">
        <div class="store-images-container">
            <img class="store-images" src="../assets/images/buy-comics-digital-comics.png">
            <p class="store-name">DIGITAL COMICS</p>
        </div>
        <div class="store-images-container">
            <img class="store-images" src="../assets/images/buy-comics-merchandise.png">
            <p class="store-name">DC MERCHANDISE</p>
        </div>
        <div class="store-images-container">
            <img class="store-images" src="../assets/images/buy-comics-subscriptions.png">
            <p class="store-name">SUBSCRIPTION</p>
        </div>
        <div class="store-images-container">
            <img class="store-images" src="../assets/images/buy-comics-shop-locator.png">
            <p class="store-name">COMIC SHOP LOCATOR</p>
        </div>
        <div class="store-images-container">
            <img class="store-images" id="power-visa-img" src="../assets/images/buy-dc-power-visa.svg">
            <p class="store-name">DC POWER VISA</p>
        </div>

    </section>


    <!-- LINK -->

    <section id="link"></section>


    <!-- FOLLOW US -->

    <section id="follow-us">
        <div id="follow-us-left">SIGN-UP NOW!</div>
        <div id="follow-us-right">
            <p id="follow-us-text">FOLLOW US</p>
            <img class="social-logo" src="../assets/images/footer-facebook.png">
            <img class="social-logo" src="../assets/images/footer-twitter.png">
            <img class="social-logo" src="../assets/images/footer-youtube.png">
            <img class="social-logo" src="../assets/images/footer-pinterest.png">
            <img class="social-logo" src="../assets/images/footer-periscope.png">
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables.scss" as *;
@use "../styles/partials/mixins.scss" as *;
@use "../styles/general.scss" as *;


#store {
    background-color: $blue-color;
    padding: 50px 18%;
    @include my-flex-row;
    gap: 50px;

    .store-images-container {

        @include my-flex-row;
        align-items: center;
        gap: 15px;

        .store-images {
            color: white;
            height: 60px;
        }

        #power-visa-img {
            width: 60px;
        }

        .store-name {
            color: white;
            font-size: 14px;
        }
    }

}

#follow-us {
    @include my-flex-row;
    justify-content: space-between;
    padding: 30px 15%;
    background-color: rgba(48, 48, 48, 255);

    #follow-us-left {
        color: white;
        padding: 13px;
        border: 2px solid rgba(2, 130, 249, 255);
        font-size: 18px;
    }

    #follow-us-right {
        @include my-flex-row;
        align-items: center;
        gap: 20px;

        #follow-us-text {
            color: rgba(2, 130, 249, 255);
            font-size: 22px;
            font-weight: 600;
        }

        .social-logo {
            height: 35px;
        }
    }
}
</style>
