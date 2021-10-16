<template>
    <div class="section-header">
        <h2>{{header}}:</h2>
        <a class="button" href="#">{{button}}</a>
    </div>
</template>

<script>
    export default {
        name: 'PopularGoodsHeader',
        data() {
            return {
                header: 'Популярные товары',
                button: 'все популярные товары'
            }
        }
    }
</script>

<style scoped>
    .section-header {
        display: flex;
        flex-flow: row nowrap;
        justify-content: space-between;
        align-items: center;
        padding: 0 30px;
    }
</style>