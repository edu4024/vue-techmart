<template>
    <div class="header">
        <Header></Header>
        <HeaderInfo></HeaderInfo>
        <SiteNavigation></SiteNavigation>
    </div>
</template>

<script>
    import Header from '../../components/mainPage/header/Header'
    import HeaderInfo from '../../components/mainPage/header/HeaderInfo'
    import SiteNavigation from '../../components/mainPage/header/SiteNavigation'
    export default {
        name: 'HeaderView',
        components: {
            Header,
            HeaderInfo,
            SiteNavigation
        }
    }
</script>

<style scoped>
    .header {
        background-color: var(--basic-grey);
        padding-bottom: 80px;
    }
</style>