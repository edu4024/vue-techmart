<template>
    <div class="section-header-wrap">
        <PopularGoodsHeader></PopularGoodsHeader>
    </div>
</template>

<script>
    import PopularGoodsHeader from '../PopularGoodsHeader'
    export default {
        name: 'SectionHeader',
        components: {
            PopularGoodsHeader
        }
    }
</script>

<style scoped>
    .section-header-wrap {
        width: 940px;
        margin: 0 auto;
        background-color: var(--basic-grey);
    }
</style>