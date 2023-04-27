<script>
export default {
    name: 'AppTestimonialsPost'
}
</script>
<template>
    <div class="my-testimonial-container">
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
    </div>
    <div class="my-latest-posts-container"></div>
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
</style>