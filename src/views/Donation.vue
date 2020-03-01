<template>
<section class="donation">
    <div class="container">
        <div class="donation__row">
            <img class="donation__img" src="@/assets/images/dog_12157.png" alt="">
            <div class="donation__infoblock">
                <div class="donation__title">
                    Кроме того, вы
                    может сделать пожертвование
                </div>
                <span class="donation__cardtitle">Наименование банка / тип банковского счета</span>
                <div class="cardlink">
                    <img src="@/assets/images/credit_card.png" alt="">
                    <div class="cardlink__number">
                        8380 2880 8028 8791 7435
                    </div>
                </div>
                <div class="donation__info">
                    Самый простой, но при этом самый эффективный способ помочь животным – это сделать пожертвование.Все ваши пожертвования бездомным животным, сделанные через наш сайт, направляются на реализацию проектов Приюта. Спасибо, что не прошли мимо и помогли тем, кто не может попросить о помощи!
                </div>
                <!-- /.donation__info -->
            </div>
            <!-- /.infoblock -->
        </div>
        <!-- /.donation__row -->
    </div>
    <!-- /.container -->
</section>
<!-- /.donation -->
</template>

<script>
    export default {
        name: "Donation"
    }
</script>

<style scoped lang="scss">
    .container{
        max-width: 925px;
        margin: 0 auto;
        padding: 0 10px 0 10px;
    }
    .donation{
        max-width: 100%;
        background-color: #f6f6f6;
        padding: 60px 0 84px 0;
        @media (max-width: 480px) {
            padding: 20px 0 20px 0;
        }
        &__row{
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }
        &__img{
            @media (max-width: 520px) {
                width: 90%;
            }
        }
        &__infoblock{
            max-width: 358px;
            width: 100%;
            display: flex;
            flex-direction: column;
        }
        &__title{
            padding-bottom: 25px;
            font-family: Georgia;
            font-size: 35px;
            line-height: 45px;
            font-weight: 400;
            letter-spacing: 0.06em;
            color: #545454;
        }
        &__cardtitle{
            padding-bottom: 13px;
            font-family: Georgia;
            font-size: 15px;
            line-height: 1.2;
            font-weight: 400;
            letter-spacing: 0.06em;
            color: #545454;
        }
        &__info{
            width: 100%;
            font-family: ArialMT;
            font-size: 12px;
            line-height: 18px;
            font-weight: 400;
            font-style: italic;
            color: #b2b2b2;
            margin-top: 33px;
        }
    }
    .cardlink{
        max-width: 319px;
        height: 47px;
        padding: 17px 14px 17px 14px;
        background-color: #f1cdb3;
        border-radius: 9px;
        text-align: center;
        display: flex;
        justify-content: space-between;
        align-items: center;
        cursor: pointer;
        &__number{
            font-family: TimesNewPSMT;
            font-size: 20px;
            line-height: 15px;
            font-weight: 400;
            letter-spacing: 0.06em;
            color: #292929;
        }
    }

</style>
