<script>
export default {
    name: "Footer"
}
</script>

<template>
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
            <img class="store-images" src="../assets/images/buy-dc-power-visa.svg">
            <p class="store-name">DC POWER VISA</p>
        </div>

    </section>
    <section id="link"></section>
    <section id="follow-us"></section>
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
        gap: 20px;

        .store-images {
            color: white;
            height: 60px;
        }

        .store-name {
            color: white;
            font-size: 14px;
        }
    }

}
</style>
