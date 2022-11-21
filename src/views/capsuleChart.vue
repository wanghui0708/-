<template>
  <!-- 胶囊柱图 -->
  <div>
    <dv-capsule-chart :config="config" style="width:100%;height:300px" />
  </div>
</template>

<script>
  export default {
    data() {
      return {
        config:{
          data: [
            {
              name: '南阳',
              value: 167
            },
            {
              name: '周口',
              value: 67
            },
            {
              name: '漯河',
              value: 123
            },
            {
              name: '郑州',
              value: 55
            },
            {
              name: '西峡',
              value: 98
            },
          ],
          colors: ['#e062ae', '#fb7293', '#e690d1', '#32c5e9', '#96bfff'],
            unit: '单位',
            showValue: true
                }
              }
            },
      }
</script>

<style lang="less" scoped>

</style>