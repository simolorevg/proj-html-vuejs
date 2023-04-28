<script>
export default {
    name: 'AppTestimonialsPost'
}
</script>
<template>
    <div class="my-testimonial-container" id="testimonials">
        <img src="../assets/img/15.png" alt="waves">
        <div class="my-testimonial-title">
            <h2>Our Testimonials</h2>
            <p>If you're planning on developing a product landing app or website, take a look at this beautiful-crafted</p>
        </div>
        <div class="my-testimonial-carousel">
            <div class="row row-cols-2">
                <div class="my-testimonial-card">
                    <i class="fa-solid fa-quote-left back-quote"></i>
                    <div class="my-card-infos">
                        <div class="d-flex flex-column justify-content-center align-items-center mb-3">
                            <img src="../assets/img/25.jpeg" alt="Mr Bean">
                            <span>
                                <em>Mac Znder</em> - Manager Softbox
                            </span>
                        </div>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas quia veniam dolore aut ad magni
                            blanditiis ea, cumque, cum modi ratione officiis maxime? Ipsa saepe veniam voluptate adipisci a
                            similique.</p>
                    </div>

                </div>
                <div class="my-testimonial-card">
                    <i class="fa-solid fa-quote-left back-quote"></i>
                    <div class="my-card-infos">
                        <div class="d-flex flex-column justify-content-center align-items-center mb-3">
                            <img src="../assets/img/26.jpeg" alt="Mr Bean">
                            <span>
                                <em>Julia Aann</em> - COO Softbox
                            </span>
                        </div>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas quia veniam dolore aut ad magni
                            blanditiis ea, cumque, cum modi ratione officiis maxime? Ipsa saepe veniam voluptate adipisci a
                            similique.</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="my-testimonial-title d-flex justify-content-center align-items-center">
            <i class="fa-solid fa-circle mx-2 text-primary"></i>
            <i class="fa-solid fa-circle"></i>
        </div>
    </div>
    <div class="my-latest-posts-container">
        <div class="d-flex flex-column justify-content-center align-items-center">
            <h3>Latest Posts</h3>
            <p>If you're planning on developing a product landing.</p>
        </div>
        <div class="row row-cols-3 d-flex justify-content-between align-items-center">
            <!--post card-->
            <div class="card my-post" style="width: 18rem;">
                <img src="../assets/img/19.jpg" class="card-img-top" alt="Clock img">
                <div class="my-post-date">4 May 2023</div>
                <div class="card-body">
                    <h5 class="card-title">Life Lack Meaning</h5>
                    <p class="card-text">
                        It's a long established fact that a reader will be distracted by the readable.
                    </p>
                </div>
            </div>
            <!--post card-->
            <!--post card-->
            <div class="card my-post" style="width: 18rem;">
                <img src="../assets/img/18.jpg" class="card-img-top" alt="Clock img">
                <div class="my-post-date">4 May 2023</div>
                <div class="card-body">
                    <h5 class="card-title">Life Lack Meaning</h5>
                    <p class="card-text">
                        It's a long established fact that a reader will be distracted by the readable.
                    </p>
                </div>
            </div>
            <!--post card-->
            <!--post card-->
            <div class="card my-post" style="width: 18rem;">
                <img src="../assets/img/17.jpg" class="card-img-top" alt="Clock img">
                <div class="my-post-date">4 May 2023</div>
                <div class="card-body">
                    <h5 class="card-title">Life Lack Meaning</h5>
                    <p class="card-text">
                        It's a long established fact that a reader will be distracted by the readable.
                    </p>
                </div>
            </div>
            <!--post card-->
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../style/general.scss' as*;

.my-testimonial-container {
    background-color: #dddad64a;

    .my-testimonial-title {
        width: 80%;
        margin: 0 auto;
        text-align: center;
        margin-bottom: 50px;
    }

    .my-testimonial-carousel {
        width: 80%;
        margin: 0 auto;

        .my-testimonial-card {
            width: calc(100% / 2 - 40px);
            background-color: white;
            margin: 20px;
            padding: 10px;
            position: relative;
            box-shadow: 20px 10px 45px 5px black;

            .back-quote {
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
                font-size: 7em;
                color: rgba(142, 142, 142, 0.178);
            }

            .my-card-infos {
                width: 100%;
                padding: 10px;
                z-index: 999;

                img {
                    border-radius: 50%;
                    width: 60px;
                    height: 60px;
                }

            }
        }
    }
}

.my-latest-posts-container {
    width: 80%;
    margin: 0 auto;
    margin-top: 80px;
    margin-bottom: 20px;

    .my-post {
        padding: 10px;
        width: calc(100% / 3 - 40px);
        margin: 0 20px;
        position: relative;
        border: 0.3px solid grey;

        .my-post-date {
            background-color: lightgray;
            color: grey;
            width: 6em;
            text-align: center;
            border-radius: 5px;
            position: absolute;
            top: 5%;
            left: 5%;
        }
    }
}
</style>