<script>
import AppBanner from './components/AppBanner.vue';
import AppHeader from './components/AppHeader.vue';
import AppTestimonialsPosts from './components/AppTestimonialsPosts.vue';
import AppTipsFeatures from './components/AppTipsFeatures.vue';

export default {
    components: {
        AppHeader,
        AppBanner,
        AppTipsFeatures,
        AppTestimonialsPosts
    },
    data() {
        return {
            tryArray: ['Hello', 'Contact Us', 'Pippo', 'Pluto', 'Paperino'],
            bannerphasesList: ['SEO', 'SEM', 'Website Strategy', 'Social Management']
        }
    }
}
</script>

<template>
    <AppHeader :linkArray=tryArray />
    <AppBanner :bannerBottom=bannerphasesList />
    <AppTipsFeatures />
    <AppTestimonialsPosts />
</template>

<style lang="scss" scoped>
@use './style/general.scss' as*;
</style>
