<template>
  <div class="home">
    <div class="wrapper">
      <div class="content">
        <hi/>
        <about/>
      </div>
    </div>
    <!-- /.wrapper -->

  </div>
</template>

<script>
import Hi from '@/views/Hi.vue'
import About from "@/views/About";
export default {
  name: 'home',
  components: {
    Hi,
    About
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
