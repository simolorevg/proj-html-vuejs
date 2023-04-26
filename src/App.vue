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
            tryArray: ['hello', 'contact us', 'pippo', 'pluto', 'paperino']
        }
    }
}
</script>

<template>
    <AppHeader :linkArray=tryArray />
    <AppBanner />
</template>

<style lang="scss" scoped>
@use './style/general.scss' as*;
</style>
