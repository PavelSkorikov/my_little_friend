<template>
  <div class="home">
    <div class="wrapper">
      <div class="content">
        <hi/>
        <main>
          <About></About>
          <Friends></Friends>
          <Help></Help>
          <Donation />
        </main>
        <Contacts />
      </div>
    </div>
  </div>
</template>

<script>
import Hi from '@/views/Hi.vue';
import About from "@/views/About";
import Friends from "@/views/Friends";
import Help from "@/views/Help";
import Donation from "@/views/Donation";
import Contacts from "@/views/Contacts";
export default {
  name: 'home',
  components: {
    Hi,
    About,
    Friends,
    Help,
    Donation,
    Contacts
  }
}
</script>

<style lang="scss">
  .wrapper {
  /* чтобы оболочка была на всю высоту экрана*/
  min-height: 100%;
  overflow: hidden;
  /*выстраиваем внутренние блоки в колонку*/
  display: flex;
  flex-direction: column;
  }
  .content {
  /*позволяем элементу увеличиваться чтобы он прижал футер к низу страницы*/
  flex: 1 1 auto;
  }
</style>
