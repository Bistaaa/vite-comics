<script>
export default {
    name: "FilmList",
    props: {
        data: Object
    }
}
</script>

<template>
    <div id="film-container">
        <div id="film-cover-container">
            <img class="film-cover" :src="data.thumb">
        </div>
        <p class="film-title">{{ data.series }}</p>
    </div>
</template>

<style lang="scss" scoped>
#film-container {

    #film-cover-container {



        .film-cover {
            height: 250px;
        }
    }


    .film-title {
        text-transform: uppercase;
    }
}
</style>

