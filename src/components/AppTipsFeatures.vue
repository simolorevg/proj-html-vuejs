<script>
export default {
    name: 'AppTipsFeatures'
}
</script>
<template>
    <div class="my-tips-container d-flex">
        <div class="my-tips-text">
            <h2 class="my-tips-title">Get tips tricks on how to skyrocket your sales.</h2>
            <p>Faff about only a quid blower I don't want no agro bleeding chimney pot burke tosser cras nice one boot
                fanny!</p>
            <div class="my-reporting-analysis">
                <div class="my-reporting-image">
                    <img src="" alt="">
                </div>
            </div>

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

    .my-tips-text {
        width: 60%;
        border: 1px solid black;

        .my-tips-title {
            width: 70%;
        }
    }

    .my-tips-image {
        flex-grow: 1;
        border: 1px solid blue;
        padding: 10px;
    }
}
</style>