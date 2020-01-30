<template>
  <div class="about">
    <div class="container">
      <div class="about__row">
        <img class="about__img" src="@/assets/images/pets_12128.png" alt="">
        <div class="about__info">
          <div class="about__title">About the shelter “Cozy House”</div>
          <div class="about__text">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi atque consectetur eius id maxime perspiciatis porro sapiente sequi. Adipisci aut debitis distinctio et iure officia quas quo. Beatae incidunt, neque?</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquam aliquid asperiores at corporis deleniti dolore, doloremque eveniet ex ipsum itaque magnam necessitatibus, non nulla odio officia omnis quasi tempora, temporibus!</p>
          </div>
        </div>
      </div>
    </div>
  </div>
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

