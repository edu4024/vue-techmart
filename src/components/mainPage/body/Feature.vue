<template>
    <section class="feature">
        <ul class="feature-list">
            <li class="feature-item">
                <div class="feature-materials">
                    <h3 class="item-header">Материаллы</h3>
                    <a class="item-link" href="#">на любой вкус</a>
                    <img class="item-icon" src="../../../assets/svg/features/icon-materials.svg" alt="materials" width="44px" height="65px">
                    <img class="item-new" src="../../../assets/img/new.png" alt="new">
                </div>
            </li>
            <li class="feature-item">
                <div class="feature-tools">
                    <h3 class="item-header">Инструмент</h3>
                    <a class="item-link" href="#">на все случаи</a>
                    <img class="item-icon" src="../../../assets/svg/features/icon-tools.svg" alt="tools" width="75px" height="61px">
                </div>
            </li>
            <li class="feature-item">
                <div class="feature-tech">
                    <h3 class="item-header">Техника</h3>
                    <a class="item-link" href="#">для стройки</a>
                    <img class="item-icon" src="../../../assets/svg/features/icon-tech.svg" alt="tech" width="78px" height="62px">
                </div>
            </li>
            <li class="feature-puncher-carusel">
                <div>
                    <img src="../../../assets/img/punchers.jpg" alt="punchers" width="620" height="266">
                    <a class="arrow left" href="#"><img src="../../../assets/svg/arrow.svg" alt="arrow"></a>
                    <a class="arrow right" href="#"><img src="../../../assets/svg/arrow.svg" alt="arrow"></a>
                    <a class="feature-puncher-carusel-btn" href="#">ОТКРЫТЬ КАТАЛОГ</a>
                </div>
            </li>
            <li class="feature-item feature-discount">
                <div class="">
                    <h3 class="item-header">Скидки 50%</h3>
                    <a class="item-link" href="#">на 350 товаров</a>
                    <img class="item-icon" src="../../../assets/svg/features/icon-discount.svg" alt="discount" width="59px" height="72px">
                </div>
            </li>
            <li class="feature-item feature-delivery">
                <div class="">
                    <h3 class="item-header">доставка</h3>
                    <a class="item-link" href="#">бесплатно</a>
                    <img class="item-icon" src="../../../assets/svg/features/icon-delivery.svg" alt="delivery" width="78px" height="63px">
                </div>
            </li>
        </ul>
    </section>
</template>

<script>
    export default {
        name: 'feature'
    }
</script>

<style scoped>
    .feature {
        background-color: var(--basic-white);
        width: 980px;
        margin: 0 auto;
    }

    .feature-list {
        list-style: none;
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        grid-row-gap: 20px;
        grid-column-gap: 10px;
        padding-left: 20px;
    }

    .feature-item {
        width: 300px;
        height: 124px;
        display: grid;
    }

    .item-header {
        color: var(--basic-white);
        margin: 10px;
    }

    .item-icon {
        right: 0px;
        padding-left: 40px;
    }

    .item-link {
        text-decoration: none;
        text-transform: uppercase;
        color: var(--basic-white);
        background-color: rgb(197, 197, 197, 0.2);
        font-size: 14px;
        line-height: 18px;
        padding: 10px;
        margin-left: 20px;
    }

    .item-link:hover {
        background-color: rgb(197, 197, 197, 0.5);
    }

    .item-link:active {
        background-color: rgb(197, 197, 197, 0.7);
    }


    .item-new {
        position: absolute;
        right: 0;
        top: 0;
    }

    .feature-materials {
        position: relative;
        background-color: #FFBF47;
        grid-column: 1/1;
        grid-row: 1/1;
    }

    .feature-tools {
        background-color: #3BBCE3;
        grid-column: 1/2;
        grid-row: 1/1;
    }

    .feature-tech {
        background-color: #DC91D8;
        grid-column: 1/3;
        grid-row: 1/1;
    }

    .feature-puncher-carusel {
        position: relative;
        width: 620px;
        height: 266px;
        grid-column: 1/3;
        grid-row: 2/3;
    }

    .feature-puncher-carusel-btn {
        position: absolute;
        text-decoration: none;
        color: var(--basic-white);
        background-color: var(--basic-red);
        width: 192px;
        height: 38px;
        bottom: 20px;
        left: 20px;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 14px;
        line-height: 18px;
    }

    .feature-puncher-carusel-btn:hover {
        background-color: var(--basic-active-red);
    }

    .feature-puncher-carusel-btn:active {
        background-color: var(--basic-active-red);
    }

    .arrow {
        position: absolute;
        text-decoration: none;
        color: var(--basic-white);
        width: 22px;
        height: 44px;
    }

    .left {
        left: 20px;
        bottom: 110px;
    }

    .right {
        right: 20px;
        bottom: 110px;
        transform: rotate(-180deg);
    }

    .feature-discount {
        background-color: #8ED78F;
        grid-column: 3;
        grid-row: 2;
    }

    .feature-delivery {
        background-color: #FFC047;
        grid-column: 3;
        grid-row: 2;
        margin-top: 140px;
    }



</style>