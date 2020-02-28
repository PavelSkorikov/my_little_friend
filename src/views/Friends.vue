<template>
<section class="friends">
    <a name="friends"></a>
    <div class="container">
        <div class="friends__col">
            <div class="friends__title">
                <span>Наши друзья, которые</span>
                <span>ищут дом</span>
            </div>
            <div class="friends__carusel">
                <Buttons @button_click="previos" label="navigate_before" black small></Buttons>
                <div class="friends__cards">
                    <Card v-for="(item, index) in cards" :key="index" :url="item.url" :name="item.name" />
                </div>
                <Buttons @button_click="next" label="navigate_next" black small />


            </div>
            <Buttons label="Познакомьтесь с остальными"  @button_click="$router.push('/contacts')" big black/>
            <!-- /.friends__carusel -->
        </div>
        <!-- /.friends__col -->

    </div>
    <!-- /.container -->
</section>
<!-- /.friends -->
</template>

<script>
    import Buttons from "../components/Buttons";
    import Card from "../components/Card";
    export default {
        name: "Friends",
        components: {
            Buttons,
            Card
        },
        data () {
            return {
                cards: [
                    { name: 'Katrine', url: 'cat_11858.png'},
                    { name: 'Jennifer', url: 'dog_11868.png'},
                    { name: 'Woody', url: 'dog_11878.png'}
                ]
            }
        },
        methods: {
            next: function () {
                this.cards.push(this.cards.shift())
            },
            previos: function () {
                this.cards.unshift(this.cards.pop())
            },
        }
    }
</script>

<style scoped lang="scss">
    .container {
        max-width: 1169px;
        margin: 0 auto;
    }
    .friends{
        max-width: 100%;
        padding: 78px 0 68px 0;
        background-color: #f6f6f6;
        @media (max-width: 1200px) {
            padding: 28px 0 28px 0;
        }
        &__col{
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            align-items: center;
        }
        &__title{
            max-width: 396px;
            text-align: center;
            font-family: Georgia;
            font-size: 35px;
            line-height: 45px;
            font-weight: 400;
            letter-spacing: 0.03em;
            color: #545454;
        }
        &__carusel{
            width: 1169px;
            margin: 26px 0 46px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
            @media (max-width: 1200px) {
                max-width: 100%;
                margin: 16px 0 16px 0;
                padding-right: 10px;
                padding-left: 10px;
            }
        }
        &__cards{
            width: 931px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            @media (max-width: 1200px) {
                max-width: 100%;
            }
            @media (max-width: 920px) {
                justify-content: center;
                :nth-child(2){
                    display: none;
                }
                :nth-child(3){
                    display: none;
                }
            }
            @media (max-width: 400px) {
                max-width: 220px;
                margin-left: 10px;
                margin-right: 10px;
            }
            @media (max-width: 330px) {
                max-width: 200px;
                margin-left: 15px;
                margin-right: 15px;
            }
        }
    }
    span{
        display: inline-block;
    }
</style>
