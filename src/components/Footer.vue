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

    <section id="link">
        <div id="link-left">

            <!-- LEFT COLUMN -->
            <div id="link-left-column">
                <h3 class="link-categories">DC COMICS</h3>
                <p class="link-titles">Characters</p>
                <p class="link-titles">Comics</p>
                <p class="link-titles">Movies</p>
                <p class="link-titles">TV</p>
                <p class="link-titles">Games</p>
                <p class="link-titles">Video</p>
                <p class="link-titles">News</p>
                <h3 class="link-categories" id="title-shop">SHOP</h3>
                <p class="link-titles">Shop DC</p>
                <p class="link-titles">Shop DC collectibles</p>
            </div>

            <!-- CENTER COLUMN -->
            <div id="link-center-column">
                <h3 class="link-categories">DC</h3>
                <p class="link-titles">Terms Of Use</p>
                <p class="link-titles">Privacy policy (New)</p>
                <p class="link-titles">Ad Choices</p>
                <p class="link-titles">Advertising</p>
                <p class="link-titles">Jobs</p>
                <p class="link-titles">Subscription</p>
                <p class="link-titles">Talent Workshops</p>
                <p class="link-titles">CPSC Certificates</p>
                <p class="link-titles">Rating</p>
                <p class="link-titles">Shop Help</p>
                <p class="link-titles">Contact Us</p>
            </div>

            <!-- RIGHT COLUMN -->
            <div id="link-right-column">
                <h3 class="link-categories">SITES</h3>
                <p class="link-titles">DC</p>
                <p class="link-titles">MAD Magazine</p>
                <p class="link-titles">DC Kids</p>
                <p class="link-titles">DC Universe</p>
                <p class="link-titles">DC Power Visa</p>
            </div>
        </div>
        <div id="link-right">
            <img id="rotated-logo" src="../assets/images/dc-logo-bg.png">
        </div>
    </section>


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

#link {
    background-image: url(../assets/images/footer-bg.jpg);
    background-size: cover;
    padding: 0 15%;
    @include my-flex-row;
    justify-content: space-between;
    align-items: center;
    height: 360px;
    overflow-y: hidden;

    #link-left {
        @include my-flex-row;
        gap: 40px;
        padding: 50px 0;

        .link-categories {
            color: white;
            margin-bottom: 15px;
        }

        .link-titles {
            color: rgba(126, 124, 124, 255);
            font-size: 13px;
            margin-bottom: 5px;
        }

        #title-shop {
            margin-top: 15px
        }
    }

    #link-right {}
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
