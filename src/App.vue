<script>
import AppBanner from './components/AppBanner.vue';
import AppHeader from './components/AppHeader.vue';

export default {
    components: {
        AppHeader,
        AppBanner
    },
    data() {
        return {
            tryArray: ['Hello', 'Contact Us', 'Pippo', 'Pluto', 'Paperino'],
            bannerObj: {
                title: 'Online Marketing',
                description: 'It is a long estabilished fact that a reader will be distraced.',
                phasesList: ['SEO', 'SEM', 'Website Strategy', 'Social Management']
            }
        }
    }
}
</script>

<template>
    <AppHeader :linkArray=tryArray />
    <AppBanner :bannerBottom=bannerObj />
</template>

<style lang="scss" scoped>
@use './style/general.scss' as*;
</style>
