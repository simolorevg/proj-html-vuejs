<script>
import AppHeader from './components/AppHeader.vue';


export default {
    components: {
        AppHeader
    },
    data() {
        return {
            tryArray: ['hello', 'contact us', 'pippo']
        }
    }
}
</script>

<template>
    <AppHeader :linkArray=tryArray />
</template>

<style lang="scss" scoped>
@use './style/general.scss' as*;
</style>
