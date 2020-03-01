<template>
  <section class="about">
    <a name="about"></a>
    <div class="container">
      <div class="about__row">
        <img class="about__img" src="@/assets/images/pets_12128.png" alt="">
        <div class="about__info">
          <div class="about__title">О приюте "Уютный дом”</div>
          <div class="about__text">
            <p>Наш приют это место содержания бездомных, потерянных или брошенных животных, преимущественно собак и кошек. Приют является одной из ключевых составляющих защиты животных и выполняют четыре основных функции: оперативная помощь и забота о животном, включая облегчение страданий посредством ветеринарной, долгосрочная забота о животном, не нашедшем немедленно старого или нового хозяина; усилия по воссоединению потерянного животного с его прежним хозяином; поиск нового места обитания или нового хозяина для бездомного животного.</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: "About",
  }
</script>

<style scoped lang="scss">
  .container {
    max-width: 834px;
    margin: 0px auto;
    padding-left: 10px;
  }
  .about{
    max-width: 100%;
    padding: 89px 0 89px 0;
    background-color: #fafafa;
    @media (max-width: 997px) {
      padding: 29px 0 29px 0;
    }
    &__row{
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
     }
    &__info{
      display: flex;
      flex-direction: column;
      max-width: 414px;
      width: 100%;
      @media (max-width: 712px) {
        padding-left: 10px;
        padding-right: 10px;
      }
    }
    &__img{
      width: 300px;
    }
    &__title{
      max-width: 300px;
      font-family: Georgia;
      font-size: 35px;
      line-height: 45px;
      font-weight: 400;
      letter-spacing: 0.03em;
      color: #545454;
      margin-bottom: 37px;
    }
    &__text{
      font-family: AriaMT;
      font-size: 15px;
      line-height: 24px;
      font-weight: 400;
      color: #4c4c4c;
    }
  }

</style>

