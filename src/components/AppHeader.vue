<script>
export default {
    name: 'AppHeader',
    props: {
        linkArray: Array
    }
}
</script>
<template>
    <div class="my-container d-flex">
        <div class="my-logo-container">
            <img src="../assets/img/logo-2.png" alt="Logo">
        </div>
        <div class="my-list-btn-container d-flex">
            <div class="my-head-list d-flex justify-content-center">
                <ul class="d-flex justify-content-start align-items-center">
                    <li v-for="(item, index) in linkArray" :key="index">
                        <a href="#link">
                            {{ item }}
                        </a>
                    </li>
                </ul>
            </div>
            <div class="my-head-btn d-flex justify-content-between align-items-center">
                <div class="my-icons d-flex justify-content-start align-items-center">
                    <i class="fa-solid fa-magnifying-glass"></i>
                    <i class="fa-solid fa-cart-shopping"></i>
                </div>
                <div class="my-btn">
                    <button type="button" class="btn btn-primary">Get Started</button>
                </div>
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
    padding: 10px 0;

    .my-logo-container {
        width: 30%;
        height: 88%;

        img {
            max-width: 100%;
            height: 100%;
        }
    }

    .my-list-btn-container {
        flex-grow: 1;
        height: 100%;

        .my-head-list {
            width: 60%;
            height: 100%;

            ul {
                list-style-type: none;
                width: 100%;
                height: 100%;

                li {
                    margin: 0 5px;
                }


                li a {
                    text-decoration: none;
                    color: inherit;

                    &:hover {
                        color: blue;
                    }
                }

            }
        }

        .my-head-btn {
            flex-grow: 1;
            height: 100%;

            .my-icons {
                width: 40%;
                height: 100%;
                gap: 20px;
                padding: 10px;
            }
        }
    }
}
</style>