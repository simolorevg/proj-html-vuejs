<script>
export default {
    name: 'AppBanner',
    props: {
        bannerBottom: Object
    }
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
    </div>
    <div class="my-banner-bottom-list">
        <div class="row">
            <div class="col d-flex">
                <div class="my-banner-icon">
                    <img src='../assets/img/24.png' alt="banner bottom image">
                </div>
                <div class="my-banner-col-text">
                    <h4>{{ bannerBottom.title }}</h4>
                    <p>{{ bannerBottom.description }}</p>
                    <ul v-for="(phase, index) in bannerBottom.phasesList" :key="index">
                        <li>{{ phase }}</li>
                    </ul>
                </div>
            </div>
            <div class="col d-flex">
                <div class="my-banner-icon">
                    <img src='../assets/img/24.png' alt="banner bottom image">
                </div>
                <div class="my-banner-col-text">
                    <h4>{{ bannerBottom.title }}</h4>
                    <p>{{ bannerBottom.description }}</p>
                    <ul v-for="(phase, index) in bannerBottom.phasesList" :key="index">
                        <li>{{ phase }}</li>
                    </ul>
                </div>
            </div>
            <div class="col d-flex">
                <div class="my-banner-icon">
                    <img src='../assets/img/24.png' alt="banner bottom image">
                </div>
                <div class="my-banner-col-text">
                    <h4>{{ bannerBottom.title }}</h4>
                    <p>{{ bannerBottom.description }}</p>
                    <ul v-for="(phase, index) in bannerBottom.phasesList" :key="index">
                        <li>{{ phase }}</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../style/general.scss' as *;

.back-color {
    background-color: #d4e1f9;
}

.my-banner-container {
    width: 95%;
    margin: 0 auto;

    .my-banner-slogan {
        width: 40%;
    }

    .my-banner-img {
        flex-grow: 1;
    }
}

.my-banner-bottom-list {
    width: 80%;
    margin: 0 auto;

    ul {
        list-style-type: none;
    }

    ul li:before {
        content: '✓';
        margin-right: 5px;
        color: blue;
    }

    .my-banner-icon {
        width: 40%;
    }

    .my-banner-col-text {
        flex-grow: 1;
    }

    .my-banner-icon,
    .my-banner-col-text {
        padding: 10px;
    }
}
</style>