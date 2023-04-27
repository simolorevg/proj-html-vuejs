<script>
export default {
    name: 'AppContactForm'
}
</script>
<template>
    <div class="my-contact-title">
        <h2>Contact our team</h2>
        <p>If you're planning on developing a product landing.</p>
    </div>
    <div class="my-contact-info d-flex">
        <div class="my-contact-map">
            <img src="../assets/img/StaticMapService.GetMapIma.png" alt="Maps">
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
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.my-contact-title {
    width: 80%;
    margin: 0 auto;
    text-align: center;
}

.my-contact-info {
    width: 80%;
    margin: 0 auto;

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