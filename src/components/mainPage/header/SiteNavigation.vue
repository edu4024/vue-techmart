<template>
    <nav class="site-navigation">
        <ul class="site-navigation-list">
            <li class="site-navigation-item"><a href="#">Главная</a></li>
            <li class="site-navigation-item"><a href="#">Компания</a></li>
            <li class="site-navigation-item"><a href="#">Каталог</a></li>
            <li class="site-navigation-item"><a href="#">Новости</a></li>
            <li class="site-navigation-item"><a href="#">Спецпредложения</a></li>
            <li class="site-navigation-item"><a href="#">Доставка</a></li>
            <li class="site-navigation-item"><a href="#">Контакты</a></li>
        </ul>
    </nav>
</template>

<script>
    export default {
        name: 'Site-navigation'
    }
</script>

<style scoped>
    ul {
        margin: 0;
        padding: 0;
    }

    .site-navigation {
        background-color: var(--basic-light-blue);
        box-shadow: inset 0px -5px 0px #293449;
        width: 940px;
        height: 60px;
        margin: 0 auto;
        padding: 0;
        flex-flow: row nowrap;
    }

    .site-navigation-list {
        display: flex;
        justify-content: space-between;
        align-items: center;
        list-style: none;
        height: 100%;
    }

    .site-navigation-item {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100%;
        width: 100%;
    }

    .site-navigation-item a {
        text-decoration: none;
        color: var(--basic-white);
        font-size: 17px;
        line-height: 17px;
    }

    .site-navigation-item:hover {
        background-color: rgba(41, 52, 73, 0.3);
    }


    .site-navigation-item:active {
        background-color: var(--basic-blue);
        color: rgba(255, 255, 255, 0.3);
    }

    .site-navigation-item a:active {
        color: rgba(255, 255, 255, 0.3);
    }
</style>