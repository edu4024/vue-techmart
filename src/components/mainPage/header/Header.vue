<template>
    <section class="header-menu">
        <div class="header-menu-wrapper">
            <ul class="header-menu-list">
                <li class="header-logo">
                    {{logo}}
                </li>
                <li class="header-menu-item">
                    <a href="#">
                        <img src="../../../assets/svg/icon-search.svg" alt="search">
                        <input type="text" placeholder="Поиск">
                    </a>
                </li>
                <li class="header-menu-item header-menu-bookmark">
                    <a href="#">
                        <img src="../../../assets/svg/icon-bookmark.svg" alt="bookmark">
                        {{bookmark}}: {{bookmarkCount}}
                    </a>
                </li>
                <li class="header-menu-item header-menu-cart">
                    <a href="#">
                        <img src="../../../assets/svg/icon-cart.svg" alt="cart">
                        {{cart}}: {{cartCount}}
                    </a>
                </li>
                <li class="header-menu-order">
                    <a href="#">Оформить заказ</a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'Header',
        data () {
            return {
                logo: 'Техномарт',
                bookmark: 'Закладки',
                bookmarkCount: 0,
                cart: 'Корзина',
                cartCount: 0
            }
        }
    }
</script>

<style scoped>
    .header-menu {
        background-color: var(--basic-blue);
        height: 42px;
    }

    .header-menu-wrapper {
        width: 940px;
        margin: 0 auto;
        padding: 0;
        flex-flow: row nowrap;
        height: 100%;
    }

    .header-menu-list {
        display: flex;
        justify-content: space-between;
        list-style: none;
        padding: 0;
        margin: 0 auto;
        height: 100%;
    }

    .header-menu-list a {
        text-decoration: none;
        color: var(--basic-white);
    }


    .header-menu-item {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100%;
        padding-left: 20px;
        padding-right: 24px;
    }

    .header-menu-item a {
       display: flex;
       justify-content: center;
       align-items: center;
    }

    .header-menu-item img {
        width: 14px;
        height: 16px;
        margin-right: 9px;
        opacity: 0.3;
    }

    .header-menu-item img:hover {
        opacity: 1;
    }

    .header-menu-bookmark:active,
    .header-menu-cart:active {
        background-color: var(--basic-active-blue);
        color: rgb(255, 255, 255, 0.3);
    }

    .header-logo {
        background-color: var(--basic-red);
        color: var(--basic-white);
        box-shadow: inset 0 -5px 0 rgba(0, 0, 0, 0.24);
        text-transform: uppercase;
        font-weight: 700;
        height: 47px;
        width: 200px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .header-logo:active {
        background-color: var(--basic-active-red);
    }

    .header-menu-order {
        background-color: var(--basic-green);
    }

    .header-menu-order a {
        height: 100%;
        padding: 0 20px;
        box-sizing: border-box;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .header-menu-order a:hover {
        background-color: var(--basic-active-green);
        color: rgb(255, 255, 255);
    }

    .header-menu-order a:active {
        background-color: var(--basic-active-green);
        opacity: 0.5;
    }

</style>