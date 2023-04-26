<script>
export default {
    name: 'AppBanner'
}
</script>
<template>
    <div class="container-fluid p-1 back-color">
        <div class="my-banner-container d-flex">
            <div class="my-banner-slogan p-3">
                <h1>The Biggest platform for your growth.</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Porro quos delectus quae temporibus excepturi
                    incidunt eius, natus repudiandae nemo sapiente optio quo beatae vel ab inventore fuga soluta sequi
                    dolores.
                </p>
                <button type="button" class="btn btn-primary">Read More</button>
            </div>
            <div class="my-banner-img">
                <img src="../assets/img/27-1.png" alt="JumboImage">
            </div>
        </div>
        <div class="my-banner-bottom-list"></div>
    </div>
</template>
<style lang="scss" scoped>
@use '../style/general.scss' as *;

.back-color {
    background-color: #c5d7f9;
}

.my-banner-container {
    width: 90%;
    margin: 0 auto;

    .my-banner-slogan {
        width: 40%;
    }
}
</style>