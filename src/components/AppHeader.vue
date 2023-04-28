<script>
export default {
    name: 'AppHeader',
    props: {
        linkArray: Object
    }
}
</script>
<template>
    <div class="my-container d-flex" id="index">
        <div class="my-logo-container">
            <a href="#home">
                <img src="../assets/img/logo-2.png" alt="Logo">
            </a>
        </div>
        <div class="my-list-btn-container d-flex">
            <div class="my-head-list d-flex justify-content-center">
                <ul class="d-flex justify-content-end align-items-center">
                    <li v-for="(item, index) in linkArray" :key="index">
                        <a :href="'#' + item.link">
                            <h5>{{ item.title }}</h5>
                        </a>
                    </li>
                </ul>
            </div>
            <div class="my-head-btn d-flex justify-content-between align-items-center">
                <div class="my-icons d-flex justify-content-start align-items-center">
                    <i class="fa-solid fa-magnifying-glass"></i>
                    <i class="fa-solid fa-cart-shopping"></i>
                    <div class="my-shopping-counter d-flex justify-content-center align-items-center">0</div>
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
            width: 70%;
            height: 100%;

            ul {
                list-style-type: none;
                width: 100%;
                height: 100%;

                li {
                    margin: 0 5px;

                    &:hover {
                        color: blue;
                        border-bottom: 2px solid blue;
                    }
                }


                li a {
                    text-decoration: none;
                    color: inherit;
                }

            }
        }

        .my-head-btn {
            flex-grow: 1;
            height: 100%;



            .my-icons {
                width: 30%;
                height: 100%;
                gap: 20px;
                padding: 10px;
                position: relative;

                i {
                    z-index: 999;
                }

                .my-shopping-counter {
                    width: 30px;
                    height: 30px;
                    background-color: #0175fb;
                    color: white;
                    border-radius: 50%;
                    position: absolute;
                    top: 0;
                    left: 80%;

                }
            }
        }
    }
}
</style>