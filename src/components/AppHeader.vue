<script>
export default {
    name: 'AppHeader',
    props: {
        link: String
    }
}
</script>
<template>
    <div class="my-container d-flex">
        <div class="my-logo-container">
            <img src="../assets/img/logo-2.png" alt="Logo">
        </div>
        <div class="my-list-btn-container d-flex">
            <div class="my-head-list d-flex justify-content-center align-items-center">
                lorem
            </div>
            <div class="my-head-btn d-flex justify-content-center align-items-center">
                lorem
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../style/general.scss' as *;

.my-container {
    width: 80%;
    height: 80px;
    margin: 0 auto;
    border: 1px solid black;

    .my-logo-container {
        width: 30%;
        height: 100%;
        border: 1px solid red;

        img {
            max-width: 100%;
            height: 100%;
        }
    }

    .my-list-btn-container {
        flex-grow: 1;
        height: 100%;
        border: 1px solid blue;

        .my-head-list {
            width: 60%;
            height: 100%;
            background-color: orange;
        }
    }
}
</style>