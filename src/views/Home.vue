<template>
  <div class="home">
    <div class="wrapper">
      <div class="content">
        <hi/>
      </div>
    </div>
    <!-- /.wrapper -->

  </div>
</template>

<script>
import Hi from '@/views/Hi.vue'
export default {
  name: 'home',
  components: {
    Hi
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
  .container{
    max-width: 1170px;
    margin: 0px auto;
  }
</style>
