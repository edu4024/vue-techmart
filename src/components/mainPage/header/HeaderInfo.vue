<template>
    <section class="header-info-wrapper">
        <ul class="header-info-list">
            <li class="header-info-item">
                <div class="header-description">
                    <p>{{description}}</p>
                </div>
            </li>
            <li class="header-info-item">
                <div class="header-contacts">
                    <div class="header-contacts-phone">
                        <img src="../../../assets/svg/icon-phone.svg" alt="ТЕЛЕФОН" width="19" height="19">
                        <a href="tel:+78125550555">{{phone}}</a>
                    </div>
                    <p class="header-contacts-adress">{{address}}</p>
                </div>
            </li>
            <li class="header-info-item">
                <ul class="header-login-list">
                    <li class="header-login-item">
                        <a href="#">
                            <img src="../../../assets/svg/icon-login.svg" alt="Войти" width="20" height="17">
                            Войти
                        </a>
                    </li>
                    <li class="header-login-item">
                        <a href="#">Регистрация</a>
                    </li>
                </ul>
            </li>
        </ul>
    </section>
</template>

<script>
    export default {
        name: 'Header-info',
        data () {
            return {
                description: 'Интернет-магазин\n' +
                    'строительных материалов\n' +
                    'и инструментов для ремонта',
                phone: '+7 (812) 555-05-55',
                address: 'г. Санкт-Петербург, ул. Б. Конюшенная, д. 19/8'
            }
        }
    }
</script>

<style scoped>
    p {
        margin: 0;
        padding: 0;
    }

    .header-info-wrapper {
        width: 940px;
        margin: 40px auto;
        flex-flow: row nowrap;
    }

    .header-info-list {
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
        list-style: none;
        width: 100%;
    }

    .header-info-item {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .header-description {
        font-size: 16px;
        line-height: 23px;
        font-style: italic;
        color: var(--basic-red);
    }

    .header-contacts-phone {
        border: 3px solid var(--basic-white);
        display: flex;
        justify-content: center;
        align-items: center;
        padding-right: 40px;
    }

    .header-contacts-phone img {
        width: 19px;
        height: 19px;
        padding-right: 40px;
    }

    .header-contacts-phone a {
        text-decoration: none;
        font-size: 21px;
        line-height: 30px;
        color: var(--basic-red);
    }

    .header-contacts p {
        text-align: center;
        padding: 0 20px;
    }

    .header-contacts-adress {
        font-size: 14px;
        line-height: 24px;
    }

    .header-login-list {
        list-style: none;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .header-login-item {
        background-color: var(--basic-white);
        border: 1px solid var(--basic-white);
        height: 100%;
        margin: 0 5px;
    }

    .header-login-item a {
        text-decoration: none;
        color: var(--basic-black);
        font-size: 21px;
        line-height: 21px;
        padding: 10px 10px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .header-login-item img {
        padding-right: 14px;
        width: 20px;
        height: 17px;
        opacity: 0.5;
    }

    .header-login-item a:hover {
        color: var(--basic-red);
    }

    .header-login-item img:hover {
        opacity: 1;
    }

    .header-login-item a:active {
        color: var(--basic-black);
        opacity: 0.3;
    }
</style>