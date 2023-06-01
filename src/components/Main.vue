<script>
export default {
    name: "Main"
}
</script>

<template>
    <div id="main-content">
        <h1>CONTENT GOES HERE</h1>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables.scss" as *;

#main-content {
    background-color: rgba(28, 28, 28, 255);

    h1 {
        color: white;
    }
}
</style>
