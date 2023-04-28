<script>
import AppBanner from './components/AppBanner.vue';
import AppContactForm from './components/AppContactForm.vue';
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppTestimonialsPosts from './components/AppTestimonialsPosts.vue';
import AppTipsFeatures from './components/AppTipsFeatures.vue';

export default {
    components: {
        AppHeader,
        AppBanner,
        AppTipsFeatures,
        AppTestimonialsPosts,
        AppContactForm,
        AppFooter
    },
    data() {
        return {
            tryArray: [
                {
                    title: 'Home',
                    link: 'home'
                },
                {
                    title: 'About Us',
                    link: 'aboutus'
                },
                {
                    title: 'Feature',
                    link: 'feature'
                },
                {
                    title: 'Testimonials',
                    link: 'testimonials'
                },
                {
                    title: 'Contact Us',
                    link: 'contactus'
                }
            ],
            bannerphasesList: ['SEO', 'SEM', 'Website Strategy', 'Social Management'],
            footObject: [
                {
                    title: 'Menu',
                    linksArray: ['About Us', 'Theme', 'Features', 'Pricing', 'Blog']
                },
                {
                    title: 'About Us',
                    linksArray: ['About Us', 'Theme', 'Features', 'Pricing', 'Blog']
                },
                {
                    title: 'Quick Links',
                    linksArray: ['About Us', 'Theme', 'Features', 'Pricing', 'Blog']
                }
            ],
            loader: true
        }
    },
    mounted() {
        this.showLoading();
        console.log(this.loader);
    },
    methods: {
        changeLoader() {
            this.loader = false;
        },
        showLoading() {
            setInterval(this.changeLoader, 4000);
        }
    }
}
</script>

<template>
    <div class="loader-container d-flex justify-content-center align-items-center" v-if="(this.loader)">
        <img src="./assets/img/loader-2.gif" alt="Loading">
    </div>
    <div v-else>
        <AppHeader :linkArray=tryArray />
        <AppBanner :bannerBottom=bannerphasesList />
        <AppTipsFeatures />
        <AppTestimonialsPosts />
        <AppContactForm />
        <AppFooter :footerObj="footObject" />
    </div>
</template>

<style lang="scss" scoped>
@use './style/general.scss' as*;

.loader-container {
    width: 100%;
    height: 100vh;
}
</style>
