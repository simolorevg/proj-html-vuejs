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
            tryArray: ['Hello', 'Contact Us', 'Pippo', 'Pluto', 'Paperino'],
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
            ]
        }
    }
}
</script>

<template>
    <AppHeader :linkArray=tryArray />
    <AppBanner :bannerBottom=bannerphasesList />
    <AppTipsFeatures />
    <AppTestimonialsPosts />
    <AppContactForm />
    <AppFooter :footerObj="footObject" />
</template>

<style lang="scss" scoped>
@use './style/general.scss' as*;
</style>
