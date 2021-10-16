<template>
    <section class="popular-goods">
        <ul class="popular-goods-list">
            <li class="popular-goods-item">
                <a class="popular-goods-img-puncher" href="#">
                    <img src="../../../assets/img/punchers/BFG900.jpg" alt="BFG900" width="184" height="164">
                </a>
                <b>Перфоратор BOSCHBFG 9000</b>
                <del>32500 Р.</del>
                <button class="button" type="button">25500 Р.</button>
            </li>
            <li class="popular-goods-item">
                <a class="popular-goods-img-puncher" href="#">
                    <img src="../../../assets/img/punchers/BFG3000.jpg" alt="BFG3000" width="127" height="112">
                </a>
                <img class="popular-goods-img-new" src="../../../assets/img/new.png" alt="new">
                <b>Перфоратор BOSCHBFG 3000</b>
                <del>22500 Р.</del>
                <button class="button" type="button">15500 Р.</button>
            </li>
            <li class="popular-goods-item">
                <a class="popular-goods-img-puncher" href="#">
                    <img src="../../../assets/img/punchers/BFG6000.jpg" alt="BFG6000" width="144" height="128">
                </a>
                <b>Перфоратор BOSCHBFG 6000</b>
                <del>30500 Р.</del>
                <button class="button" type="button">25500 Р.</button>
            </li>
            <li class="popular-goods-item">
                <a class="popular-goods-img-puncher" href="#">
                    <img src="../../../assets/img/punchers/BFG2000.jpg" alt="BFG2000" width="127" height="112">
                </a>
                <img class="popular-goods-img-new" src="../../../assets/img/new.png" alt="new">
                <b>Перфоратор BOSCHBFG 2000</b>
                <del>22500 Р.</del>
                <button class="button" type="button">12500 Р.</button>
            </li>
        </ul>
    </section>
</template>

<script>
    export default {
        name: 'PopularGoods'
    }
</script>

<style scoped>

    .popular-goods {
        width: 940px;
        margin: 0 auto;
        padding: 0;
        margin-top: 50px;
    }

    .popular-goods-list {
        list-style: none;
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-gap: 20px;
        justify-items: center;
    }

    .popular-goods-item {
        display: grid;
        justify-items: center;
        grid-template-rows: 150px repeat(auto-fill, minmax(18px, 41px));
        grid-gap: 10px;
        border: 1px solid var(--basic-grey);
    }

    b {
        font-size: 18px;
        line-height: 20px;
        font-family: 'PT Sans', sans-serif;
        text-align: center;
    }

    .popular-goods-img-puncher {
        display: block;
        margin-top: 20px;
    }

    .popular-goods-img-new {
        position: relative;
        left: 70px;
        bottom: 160px;
    }
</style>