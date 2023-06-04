<script>
export default {
    name: "Header"
}
</script>

<template>
    <div id="header-content">
        <img id="logo" src="../assets/images/dc-logo.png">

        <nav>
            <div id="characters" class="nav-container">
                <p class="nav-buttons">CHARACTERS</p>
                <hr>
            </div>
            <div id="comics" class="nav-container">
                <p class="nav-buttons">COMICS</p>
                <hr>
            </div>
            <div id="movies" class="nav-container">
                <p class="nav-buttons">MOVIES</p>
                <hr>
            </div>
            <div id="tv" class="nav-container">
                <p class="nav-buttons">TV</p>
                <hr>
            </div>
            <div id="games" class="nav-container">
                <p class="nav-buttons">GAMES</p>
                <hr>
            </div>
            <div id="collectibles" class="nav-container">
                <p class="nav-buttons">COLLECTIBLES</p>
                <hr>
            </div>
            <div id="videos" class="nav-container">
                <p class="nav-buttons">VIDEOS</p>
                <hr>
            </div>
            <div id="fans" class="nav-container">
                <p class="nav-buttons">FANS</p>
                <hr>
            </div>
            <div id="news" class="nav-container">
                <p class="nav-buttons">NEWS</p>
                <hr>
            </div>
            <div id="shop" class="nav-container">
                <p class="nav-buttons">SHOP</p>
                <hr>
            </div>
        </nav>

    </div>

    <div id="jumbotron_container">
        <!-- <img id="jumbotron" src="../assets/images/jumbotron.jpg"> -->
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/general.scss" as *;
@use "../styles/partials/variables.scss" as *;
@use "../styles/partials/mixins.scss" as *;

#header-content {
    @include my-flex-row;
    justify-content: space-between;
    align-items: flex-end;
    padding: 0 15%;

    #logo {
        margin: 10px 0;
        height: 80px
    }

    nav {
        @include my-flex-row;
        gap: 30px;

        .nav-buttons {
            padding: 30px 0;
        }

        hr {
            width: 70%;
            border: 2px solid white;
        }



        .nav-container:hover {
            .nav-buttons {
                color: $blue-color;
                cursor: pointer;
            }

            .nav-container hr {
                border: 2px solid $blue-color;
            }
        }
    }
}

#jumbotron_container {
    height: 400px;
    background-image: url(../assets/images/jumbotron.jpg);
    background-size: cover;
    background-repeat: no-repeat;
}
</style>
