<template>
    <header class="hi">
        <img src="../assets/images/dog_12173.png" alt="" class="hi__img">
        <div class="container">
            <div class="hi__row">
                <div class="hi__col-1">
                    <p class="hi__title">
                        <span class="hi__name">Уютный дом</span>
                        <span class="hi__subname">Приют для домашних животных в Ростове на Дону</span>
                    </p>
                    <div class="hi__info">
                        <p class="hi__slogan">
                            Не только людям нужен дом
                        </p>
                        <p class="hi__annotate">Мы хотим, чтобы как можно больше людей, завели дома кошку или собаку из приюта. Потому что этот процесс затрагивает не только спасение животных, но и формирует в людях милосердие, они мгновенно получают мощный заряд положительной энергии и любви.</p>
                        <Buttons label="Завести друга" @button_click="$router.push('/friends')"/>
                    </div>
                </div>
                <div class="hi__col-2">
                    <nav class="hi__navbar">
                        <Navbar></Navbar>
                    </nav>
                </div>
            </div>
        </div>
    </header>
</template>

<script>
    import Buttons from '@/components/Buttons.vue'
    import Navbar from "../components/Navbar";
    export default {
        name: "Hi",
        components: {
            Buttons,
            Navbar
        }
    }
</script>

<style scoped lang="scss">
    .container{
        max-width: 1170px;
        margin: 0px auto;
    }
    .hi {
        max-width: 100%;
        height: 925px;
        padding-top: 60px;
        background: url(../assets/images/background.jpg) no-repeat;
        background-size: cover;
        @media (max-width: 1024px){
            padding-top: 10px;
            height: 750px;
        }
        @media (max-width: 800px){
            padding-top: 10px;
            height: 500px;
        }
        &__row {
            display: flex;
            flex-wrap: wrap-reverse;
        }
        &__col-1 {
            padding: 0 0 10px 10px;
            display: flex;
            flex-direction: column;
            flex: 1 1 50%;
        }
        &__col-2 {
            padding: 0 0 10px 10px;
            margin-bottom: 30px;
            display: flex;
            flex-direction: column;
            flex: 1 1 50%;
            flex-wrap: wrap;
        }
        &__title {
            max-width: 210px;
            margin-bottom: 250px;
            @media (max-width: 1180px){
               margin-bottom: 50px;
            }
        }
        &__name {
            display: inline-block;
            font-family: georgia;
            font-size: 32px;
            line-height: 42px;
            font-weight: 400;
            letter-spacing: 0.033em;
            color: #f1cdb3;
        }
        &__subname {
            display: inline-block;
            font-family: ArialMT;
            font-size: 13px;
            line-height: 21px;
            font-weight: 400;
            letter-spacing: 0.13em;
            color: #ffffff;
        }
        &__info {
            max-width: 443px;
            margin-bottom: 44px;
        }
        &__slogan {
            max-width: 400px;
            font-family: Georgia;
            font-size: 44px;
            line-height: 57px;
            font-weight: 300;
            letter-spacing: 0.05em;
            color: #ffffff;
            @media (max-width: 780px){
                font-size: 24px;
                line-height: 27px;
            }
        }
        &__annotate {
            margin-bottom: 24px;
            font-family: ArialMT;
            font-size: 15px;
            line-height: 24px;
            font-weight: 400;
            color: #cdcdcd;
        }
        &__navbar {
            display: flex;
            justify-content: flex-end;
            @media (max-width: 1180px){
                justify-content: flex-start;
            }
            @media (max-width: 750px){
                max-width: 250px;
            }
            @media (max-width: 300px){
                max-width: 150px;
            }
        }
        &__img {
            position: absolute;
            top: 0;
            left: 950px;
            display: block;
            max-width: 100%;
            @media (max-width: 1618px){
                left: 720px;
            }
            @media (max-width: 1400px){
                left: 520px;
            }
            @media (max-width: 1180px){
                width: 50%;
                top: 50px;
                left: 450px;
            }
            @media (max-width: 900px){
                width: 40%;
                left: 400px;
            }
            @media (max-width: 700px){
                left: 330px;
            }
            @media (max-width: 530px){
            display: none;
            }
            @media (min-width: 2300px){
                left: 1300px;
            }
            @media (min-width: 2900px){
                left: 1800px;
            }

        }

    }

</style>
