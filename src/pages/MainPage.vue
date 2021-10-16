<template>
    <div class="main">
        <HeaderView></HeaderView>
        <bodyView></bodyView>
    </div>
</template>

<script>
    import HeaderView from '../views/header/HeaderView'
    import bodyView from '../views/body/bodyView'
    export default {
        name: 'main-page',
        components: {
            HeaderView,
            bodyView
        }
    }
</script>

<style>
    :root {
        --basic-red: #EE3643;
        --basic-active-red: #BA2732;
        --basic-green: #63A63E;
        --basic-active-green: #5FBB2D;
        --basic-blue: #293449;
        --basic-light-blue: #32425C;
        --basic-active-blue: #1D2739;
        --basic-black: #000000;
        --basic-gold: #FFD180;
        --basic-grey: #F3F7F9;
        --basic-light-grey: #C5C5C5;
        --basic-white: #FFFFFF;
    }

    .main {
        margin: 0;
        padding: 0;
        font-family: 'Cuprum', sans-serif;
        min-width: 940px;
        color: var(--basic-black);
        background-color: var(--basic-white);
        background-position: center;
        background-repeat: no-repeat;
    }

    h2 {
        font-size: 30px;
        line-height: 30px;
    }

    img {
        max-width: 100%;
        height: auto;
    }

    .button {
        font: inherit;
        font-size: 14px;
        line-height: 18px;
        color: var(--basic-white);
        vertical-align: middle;
        text-decoration: none;
        background-color: var(--basic-red);
        border: none;
        text-transform: uppercase;
        width: 192px;
        height: 38px;
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>