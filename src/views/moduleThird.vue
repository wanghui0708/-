<template>
  <!-- 第三行 -->
  <div class="module-box">
        <div style="flex:0 1 50%">
          <dv-border-box-8 style="width:100%;height: 300px ;">
            <bar-charts></bar-charts>
          </dv-border-box-8>
        </div>
        <div style="flex:0 1 25%">
          <dv-border-box-8 style="width:100%;height: 300px ;">
            <dv-active-ring-chart :config="config1" style="width:100%;height:300px" />
          </dv-border-box-8>
        </div>
        <div style="flex:0 1 25%">
          <dv-border-box-8 style="width:100%;height: 300px ;">
          <line-chart></line-chart>
          </dv-border-box-8>
        </div>
      </div>
</template>

<script>
import BarCharts from './barCharts.vue'
import lineChart from './lineChart.vue'
  export default {
  components: { lineChart ,BarCharts},
  data() {

        return {
      config1:{
        data: [
                {
                  name: '周口',
                  value: 55
                },
                {
                  name: '南阳',
                  value: 120
                },
                {
                  name: '西峡',
                  value: 78
                },
                {
                  name: '驻马店',
                  value: 66
                },
                {
                  name: '新乡',
                  value: 80
                }
              ]
                  }
                }
              },
  }
</script>

<style lang="less" scoped>

</style>