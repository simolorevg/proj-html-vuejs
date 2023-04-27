<script>
export default {
    name: 'AppFooter',
    props: {
        footerObj: Object
    }
}
</script>
<template>
    <div class="my-footer-container">
        <div class="my-footer-list d-flex">
            <div class="my-footer-agency">
                <img src="../assets/img/35.png" alt="Logo Agency">
            </div>
            <div class="my-footer-links">
                <div class="row row-cols-3">
                    <div class="col my-footer-link" v-for="(link, index) in footerObj" :key="index">
                        <h4>{{ footerObj[index].title }}</h4>
                        <ul>
                            <li v-for="(link, index) in footerObj[index].linksArray" :key="index">
                                <a href="#link">
                                    {{ link }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="my-gtt-btn">
                <div class="my-gtt-color">
                    <a href="#index">
                        <i class="fa-solid fa-chevron-up"></i>
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../style/general.scss' as *;

.my-footer-container {
    width: 100%;
    border-top: 1px solid grey;

    .my-footer-list {
        width: 80%;
        margin: 0 auto;

        .my-footer-agency {
            width: 20%;
        }

        .my-footer-links {
            flex-grow: 1;

            .my-footer-link {
                width: calc(100% / 3 - 40px);
                margin: 0 20px;

                ul li {
                    list-style-type: none;

                    a {
                        text-decoration: none;
                        color: inherit;
                    }
                }
            }
        }

        .my-gtt-btn {
            width: 10%;
            position: relative;

            .my-gtt-color {
                width: 40px;
                height: 40px;
                border-radius: 50%;
                background-color: grey;
                color: white;
                display: flex;
                justify-content: center;
                align-items: center;
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);

                a {
                    color: inherit;
                }
            }
        }
    }
}
</style>