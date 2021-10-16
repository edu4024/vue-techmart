<template>
    <div>
        <Feature></Feature>
        <SectionHeader></SectionHeader>
        <PopularGoods></PopularGoods>
    </div>
</template>

<script>
    import Feature from '../../components/mainPage/body/Feature'
    import SectionHeader from '../../components/mainPage/body/sections/SectionHeader'
    import PopularGoods from '../../components/mainPage/body/PopularGoods'
    export default {
        name: 'bodyView',
        components: {
            Feature,
            SectionHeader,
            PopularGoods
        }
    }
</script>

<style scoped>

</style>