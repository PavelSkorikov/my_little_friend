<template>
    <div class="hi">
        <!-- /.hi__img -->
        <div class="container">
            <div class="hi__row">
                <div class="hi__col">
                    <p class="hi__title">
                        <span class="hi__name">Cozy House</span>
                        <span class="hi__subname">Shelter for pets in Boston</span>
                    </p>
                    <div class="hi__info">
                        <p class="hi__slogan">
                            Not only people need a house
                        </p>
                        <p class="hi__annotate">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquid debitis esse ipsam iste nostrum possimus provident quae quo repudiandae, similique, tempore unde. Aperiam odit optio reprehenderit voluptates! Minima, possimus, voluptas!</p>
                        <Button label="Make a friend"/>
                    </div>
                </div>
                <div class="hi__col">
                    <Navbar></Navbar>
                    <img src="../assets/images/dog_12173.png" alt="" class="hi__img">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import Button from '@/components/Button.vue'
    import Navbar from "../components/Navbar";
    export default {
        name: "Hi",
        components: {
            Button,
            Navbar
        }
    }
</script>

<style scoped lang="scss">
    .hi {
        max-width: 100%;
        height: 925px;
        padding-top: 60px;
        background-image: url(../assets/images/background_12165.png);
        &__row {
            display: flex;
        }
        &__col {
            display: flex;
            flex-direction: column;
            flex: 1 1 50%;
        }
        &__title {
            max-width: 181px;
            margin-bottom: 250px;
            @media (max-width: 1180px){
               margin-bottom: 50px;
            }
        }
        &__name {
            display: inline-block;
            font-family: georgia;
            font-size: 32px;
            line-height: 29px;
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
            max-width: 346px;
            font-family: Georgia;
            font-size: 44px;
            line-height: 57px;
            font-weight: 300;
            letter-spacing: 0.05em;
            color: #ffffff;
            @media (max-width: 680px){
                font-size: 24px;
                line-height: 27px;
            }
        }
        &__annotate {
            margin-bottom: 44px;
            font-family: ArialMT;
            font-size: 15px;
            line-height: 24px;
            font-weight: 400;
            color: #cdcdcd;
        }
        &__img {
            position: absolute;
            top: 0;
            left: 950px;
            @media (max-width: 1618px){
                left: 720px;
            }
            @media (max-width: 1400px){
                left: 520px;
            }
            @media (max-width: 1180px){
                width: 50%;
                top: 100px;
            }
            @media (max-width: 750px){
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
