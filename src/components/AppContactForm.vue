<script>
export default {
    name: 'AppContactForm'
}
</script>
<template>
    <div class="my-contact-title" id="contactus">
        <h2>Contact our team</h2>
        <p>If you're planning on developing a product landing.</p>
    </div>
    <div class="my-contact-info d-flex">
        <div class="my-contact-map">
            <img src="../assets/img/StaticMapService.GetMapIma.png" alt="Maps">
            <div class="my-map-info d-flex">
                <div class="d-flex flex-column">
                    <h5>Storey Ave</h5>
                    <p>San Francisco, California 94129</p>
                    <a href="#maps" class="my-2">Visualizza la mappa più grande</a>
                </div>
                <div class="my-map-icon d-flex flex-column mx-4">
                    <i class="fa-regular fa-compass fs-1"></i>
                    <a href="#direction" class="my-4">Indicazioni</a>
                </div>
            </div>
        </div>
        <div class="my-contact-form mx-3">
            <div class="my-contact-address">
                <img src="../assets/img/35.png" alt="Agency Logo my-2">
                <h3 class="my-3">9840 Shore St. Fond Du Lac, WI 54935</h3>
                <p class="my-2">0 1223 456 789</p>
                <p class="my-2">mail@sofbox.com</p>
            </div>
            <div class="my-contact-input">
                <h3>Get in Touch</h3>
                <div class="d-flex justify-space-between my-2">
                    <label for="client-name d-none"></label>
                    <input type="text" id="client-name" placeholder="Your Name">
                    <label for="client-email d-none"></label>
                    <input type="email" id="client-email" placeholder="Your Email" class="mx-2">
                </div>
                <label for="client-subject d-none"></label>
                <input type="text" id="client-subject" placeholder="Your Subject" class="my-3">
                <label for="client-message d-none"></label>
                <textarea name="" id="client-message" cols="60" rows="10" placeholder="Your Message Here"></textarea>
                <button type="button" class="btn btn-primary my-3">Send Message</button>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../style/general.scss' as*;

.my-contact-title {
    width: 80%;
    margin: 0 auto;
    text-align: center;
}

.my-contact-info {
    width: 80%;
    margin: 0 auto;

    .my-contact-map {
        position: relative;

        .my-map-info {
            position: absolute;
            background-color: white;
            top: 2%;
            left: 3%;
            padding: 10px;

            a {
                text-decoration: none;
                font-size: 0.6em;
            }
        }
    }

    .my-contact-form {
        padding: 10px;

        #client-name {
            width: 60%;
        }

        #client-email {
            flex-grow: 1;
        }

        #client-subject {
            width: 100%;
        }
    }
}
</style>