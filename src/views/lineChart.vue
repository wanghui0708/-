<template>
  <div ref="chart" style="width: 100%;height:300px;"></div>
</template>

<script>
import * as echarts from 'echarts/core'

  export default {
    data() {
      return {
        
      }
    },
    mounted(){
      this.initChart()
    
    },
    methods:{
      initChart(){
         // 基于准备好的dom，初始化echarts实例
      var myChart = echarts.init(this.$refs.chart);

        // 指定图表的配置项和数据
        var option = {
         
          legend: {
            data: ['销量']
          },
          xAxis: {
            data: ['衬衫', '羊毛衫', '雪纺衫', '裤子', '高跟鞋', '袜子', '裤子', '高跟鞋', '袜子']
          },
          yAxis: {},
          series: [
            {
              name: '销量',
              type: 'line',
              data: [5, 20, 36, 10, 10, 20,32,43,21]
            }
          ]
        };

        // 使用刚指定的配置项和数据显示图表。
        myChart.setOption(option);
      },
      
    }
  }
</script>

<style lang="less" scoped>

</style>