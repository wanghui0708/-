<template>
<!-- 第一行 -->
<div class="module-box">
        <div style="flex:0 1 30%">
          <dv-decoration-10 style="width:90%;height:5px;" />
        </div>
        <div style="flex:0 1 40%">
          <div class="d-flex">
            <dv-decoration-8 style="height:50px; flex:1" />
            <div class="tc .box-middle" style="flex:1">
              <dv-decoration-11 style="height:60px;">智慧数据中心</dv-decoration-11>
            </div>
            <dv-decoration-8 :reverse="true" style="height:50px;flex:1" />
          </div>

        </div>
        <div style="flex:0 1 30%">
          <dv-decoration-10 style="width:90%;height:5px; transform: rotate(180deg);" />
        </div>
      </div>
</template>

<script>
  export default {
    
  }
</script>

<style lang="less" scoped>

</style>