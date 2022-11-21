<template>
  <div class="content bg">
    <!-- 全屏容器 -->
    <dv-full-screen-container>
      <!-- 第一行 -->
      <module-title></module-title>
      <!-- 第二行 -->
      <module-main></module-main>
      <!-- 第三行 -->
     <module-third></module-third>
    </dv-full-screen-container>
  </div>
</template>

<script>
import ModuleMain from './moduleMain.vue'
import ModuleThird from './moduleThird.vue'
import ModuleTitle from './moduleTitle.vue'
  export default {
    name:'HomeView',
    components:{
      ModuleTitle,
      ModuleMain,
      ModuleThird
    },
    data() {
      return { }
    },
  }
</script>

<style lang="less" scoped>

</style>