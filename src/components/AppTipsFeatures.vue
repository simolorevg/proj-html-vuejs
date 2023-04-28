<script>
export default {
    name: 'AppTipsFeatures',
    data() {
        return {
            hoverCol: false
        }
    }
}
</script>
<template>
    <div class="my-tips-container d-flex" id="aboutus">
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
                    <img src="../assets/img/511.png" alt="Graph Image">
                </div>
                <div class="my-reporting-text">
                    <h3>Technical SEO Audit</h3>
                    <p>It is a long established fact that a reader will be distracted by the readble content of a page, when
                        looking at its layout.</p>
                </div>
            </div>
        </div>
        <div class="my-tips-image">
            <img src="../assets/img/509.jpeg" alt="Team Tips">
        </div>
    </div>
    <div class="my-design-feature-container">
        <img class="design-ball" src="../assets/img/14.png" alt="design ball">
        <div class="my-features-container">
            <div class="my-features-intro d-flex">
                <div class="my-features-title" id="feature">
                    <h3>Popular features that your business needs</h3>
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Incidunt porro aperiam recusandae unde
                        adipisci
                        tenetur beatae quos architecto. Quod, sint rerum? Ullam vero unde culpa consequuntur, atque iusto
                        nostrum. Vero.</p>
                </div>
                <div class="my-features-cta d-flex align-items-center">
                    <button type="button" class="btn btn-primary">Explore More Features</button>
                </div>
            </div>
            <div class="my-features-columns">
                <div class="row row-cols-4 p-4 d-flex justify-content-center">
                    <div class="my-card-col blue">
                        <p class="card-title">Customized Invoices</p>
                        <i class="fa-solid fa-chart-line fs-1 "></i>
                        <i class="fa-solid fa-braille fs-1"></i>
                    </div>
                    <div class="my-card-col red">
                        <p class="card-title">Stock Management</p>
                        <i class="fa-regular fa-paper-plane fs-1 "></i>
                        <i class="fa-solid fa-braille fs-1"></i>
                    </div>
                    <div class="my-card-col green">
                        <p class="card-title">Receivable & Payables</p>
                        <i class="fa-solid fa-award fs-1 "></i>
                        <i class="fa-solid fa-braille fs-1"></i>
                    </div>
                    <div class="my-card-col blue">
                        <p class="card-title">Manage Buying</p>
                        <i class="fa-solid fa-chalkboard-user fs-1 "></i>
                        <i class="fa-solid fa-braille fs-1"></i>
                    </div>
                    <div class="my-card-col red">
                        <p class="card-title">Powerful & Secure</p>
                        <i class="fa-solid fa-network-wired fs-1"></i>
                        <i class="fa-solid fa-braille fs-1"></i>
                    </div>
                    <div class="my-card-col green">
                        <p class="card-title">Fastest Return Filing</p>
                        <i class="fa-solid fa-stopwatch fs-1 "></i>
                        <i class="fa-solid fa-braille fs-1"></i>
                    </div>
                    <div class="my-card-col blue">
                        <p class="card-title">Monthly Detailed</p>
                        <i class="fa-solid fa-file-signature fs-1 "></i>
                        <i class="fa-solid fa-braille fs-1"></i>
                    </div>
                    <div class="my-card-col red">
                        <p class="card-title">Product Management</p>
                        <i class="fa-regular fa-thumbs-up fs-1"></i>
                        <i class="fa-solid fa-braille fs-1"></i>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../style/general.scss' as*;

.my-tips-container {
    width: 80%;
    margin: 0 auto;
    margin-top: 80px;

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

    .my-reporting-analysis:nth-child(even) {
        background: rgb(227, 227, 227);
        background: linear-gradient(180deg, rgba(227, 227, 227, 1) 0%, rgba(255, 255, 255, 1) 35%);
    }

    .my-tips-image {
        flex-grow: 1;
        padding: 10px;
    }
}

.my-design-feature-container {
    width: 100%;
    position: relative;

    .design-ball {
        position: absolute;
        top: -5%;
        left: -38%;
    }
}

.my-features-container {
    width: 80%;
    margin: 0 auto;

    .my-features-title {
        width: 60%;
        padding: 10px;
    }

    .my-features-cta {
        flex-grow: 1;
        padding: 10px;
    }

    .my-features-columns {
        width: 100%;


        .fa-solid:hover,
        .fa-regular:hover {
            color: inherit;
        }

        .red:hover {
            background: rgb(255, 166, 166);
            background: linear-gradient(208deg, rgba(255, 166, 166, 1) 0%, rgba(254, 0, 0, 1) 35%);
            color: white;

            .fa-braille {
                display: inline;
                color: red;
                z-index: -10;
            }

        }

        .green:hover {
            background: rgb(183, 255, 166);
            background: linear-gradient(208deg, rgba(183, 255, 166, 1) 0%, rgba(0, 254, 38, 1) 35%);
            color: white;

            .fa-braille {
                display: inline;
                color: green;
                z-index: -10;
            }
        }

        .blue:hover {
            background: rgb(101, 114, 255);
            background: linear-gradient(208deg, rgba(101, 114, 255, 1) 0%, rgba(0, 18, 254, 1) 35%);
            color: white;

            .fa-braille {
                display: inline;
                color: blue;
                z-index: -10;
            }
        }
    }

    .my-card-col {
        width: calc(100% / 4 - 40px);
        background-color: white;
        padding: 20px;
        margin: 20px;
        box-shadow: -1px -3px 42px -13px rgba(0, 0, 0, 0.75);
        position: relative;


        .fa-braille {
            position: absolute;
            bottom: -10%;
            right: -10%;
            transform: rotate(180deg);
            display: none;
        }



        .card-title {
            margin-bottom: 30px;
            font-size: 1.1rem;
        }
    }
}
</style>