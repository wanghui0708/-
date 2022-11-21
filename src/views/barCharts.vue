<template>
  <div>
    <div ref="chart" style="width: 100%;height:300px;"></div>
  </div>
</template>

<script>
import * as echarts from 'echarts/core'
  export default {
    mounted(){
      this.initChart()
    },
    methods:{
      initChart(){
        var myChart=echarts.init(this.$refs.chart)
        // 指定图表的配置项和数据
      var option = {
        xAxis: {
    data: ['A', 'B', 'C', 'D', 'E']
  },
  yAxis: {},
  series: [
    {
      type: 'bar',
      data: [23, 24, 18, 25, 18],
      barGap: '20%',
      barCategoryGap: '40%'
    },
    {
      type: 'bar',
      data: [12, 14, 9, 9, 11]
    }
  ]
      };
      myChart.setOption(option);
      }
    }
  }
</script>

<style lang="less" scoped>

</style>