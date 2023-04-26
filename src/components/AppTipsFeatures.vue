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
            <div class="my-reporting-analysis d-flex align-items-center">
                <div class="my-reporting-image">
                    <img src="../assets/img/510.png" alt="Repo Image">
                </div>
                <div class="my-reporting-text">
                    <h3 class="my-repo-title">Reporting Analysis</h3>
                    <p>It is a long established fact that a reader will be distracted by the readble content of a page, when
                        looking at its layout.</p>
                </div>
            </div>
            <div class="my-reporting-analysis d-flex align-items-center">
                <div class="my-reporting-image">
                    <img src="../assets/img/510.png" alt="Repo Image">
                </div>
                <div class="my-reporting-text">
                    <h3>Reporting Analysis</h3>
                    <p>It is a long established fact that a reader will be distracted by the readble content of a page, when
                        looking at its layout.</p>
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

        .my-tips-title {
            width: 70%;
        }
    }

    .my-reporting-analysis {
        margin: 50px 0;

        .my-repo-title {
            color: blue;
        }

        .my-reporting-image {
            width: 20%;

            img {
                width: 50px;
                height: 50px;
            }
        }

        .my-reporting-text {
            flex-grow: 1;
        }
    }

    .my-tips-image {
        flex-grow: 1;
        padding: 10px;
    }
}
</style>