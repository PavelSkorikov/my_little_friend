<template>
  <div class="home">
    <div class="wrapper">
      <div class="content">
        <hi/>
        <about/>
        <Our_friends />
        <Help />
        <Donation />
      </div>
    </div>
    <!-- /.wrapper -->

  </div>
</template>

<script>
import Hi from '@/views/Hi.vue';
import About from "@/views/About";
import Our_friends from "./Our_friends";
import Help from "./Help";
import Donation from "./Donation";
export default {
  name: 'home',
  components: {
    Hi,
    About,
    Our_friends,
    Help,
    Donation
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
