<script>
export default {
    name: 'AppTipsFeatures'
}
</script>
<template>
    <div class="my-tips-container d-flex">
        <div class="my-tips-text">
            Lorem
        </div>
        <div class="my-tips-image">
            <img src="../assets/img/509.jpeg" alt="Team Tips">
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../style/general.scss' as*;

.my-tips-container {
    width: 80%;
    margin: 0 auto;
    border: 1px solid red;

    .my-tips-text {
        width: 60%;
        border: 1px solid black;
    }

    .my-tips-image {
        flex-grow: 1;
    }
}
</style>