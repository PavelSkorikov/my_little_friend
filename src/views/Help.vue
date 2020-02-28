<template>
    <section class="help">
        <a name="help"></a>
        <div class="container">
            <div class="help__col">
                <div class="help__title">
                    Чем вы можете помочь нашему приюту
                </div>
                <div class="help__row1">
                    <Infobanner v-for="(item, index) in banners.slice(0, 5)" :key="index" :info="item.info" :url="item.url" />
                </div>
                <div class="help__row2">
                    <Infobanner v-for="(item, index) in banners.slice(5, 9)" :key="index" :info="item.info" :url="item.url" />
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    import Infobanner from "@/components/Infobanner";
    export default {
        name: "Help",
        components: {
            Infobanner
        },
        data () {
            return {
                banners: [
                    {info: 'Корм', url: 'cat_food_11363.png'},
                    {info: 'Перевозка', url: 'ambulance_11347.png'},
                    {info: 'Игрушки', url: 'ball_11354.png'},
                    {info: 'Миски и чашки', url: 'bowl_11361.png'},
                    {info: 'Шампуни', url: 'shampoo_11370.png'},
                    {info: 'Витамины', url: 'pills_11446.png'},
                    {info: 'Медикаменты', url: 'syringe_11448.png'},
                    {info: 'Ошейники / поводки', url: 'leash_11450.png'},
                    {info: 'Зона отдыха', url: 'cat_11456.png'},
                ]
            }
        }
    }
</script>

<style scoped lang="scss">
    .container{
        max-width: 1023px;
        margin: 0 auto;
    }
    .help{
        max-width: 100%;
        padding: 72px 0 83px 0;
        background-color: #fafafa;
        @media (max-width: 480px) {
            padding: 20px 0 20px 0;
        }
        &__col{
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        &__title{
            max-width: 316px;
            margin-bottom: 82px;
            font-family: Georgia;
            font-size: 35px;
            line-height: 45px;
            font-weight: 400;
            letter-spacing: 0.03em;
            color: #545454;
            text-align: center;
            @media (max-width: 414px) {
                margin-bottom: 20px;
            }
        }
        &__row1{
            width: 100%;
            padding: 0 10px 0 10px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            @media (max-width: 360px) {
                justify-content: space-around;
            }
        }
        &__row2{
            margin-top: 79px;
            width: 80%;
            padding: 0 10px 0 10px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            @media (max-width: 414px) {
                width: 100%;
                margin-top: 10px;
                justify-content: space-around;
            }
        }
    }
</style>
