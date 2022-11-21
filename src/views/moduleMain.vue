<template>
 <div class="module-box">
        <!-- 左 -->
        <div style="flex:0 1 25%">
          <dv-border-box-8 style="width:100%;height: 200px ;">
            <dv-capsule-chart :config="config1" style="width:100%;height:200px" />
          </dv-border-box-8>
          <dv-border-box-2 style="width:100%;height: 200px ;">
            <dv-water-level-pond :config="config3" style="width:100%;height:200px" />
          </dv-border-box-2>
          <dv-border-box-2 style="width:100%;height: 200px ;">
            <dv-conical-column-chart :config="config5" style="width:100%;height:200px;" />
          </dv-border-box-2>
        </div>
        <!-- 中 -->
        <div style="flex:0 1 50%">
          <dv-border-box-6 style="width:100%;height: 600px ;">
            <dv-flyline-chart :config="config4" style="width:100%;height:100%;" />
          </dv-border-box-6>
        </div>
        <!-- 右 -->
        <div style="flex:0 1 25%">
          <dv-border-box-5 style="width:100%;height: 300px ;">
            <capsule-chart></capsule-chart>
          </dv-border-box-5>
          <dv-border-box-8 style="width:100%;height: 300px ;">
            <dv-scroll-ranking-board :config="config2" style=" width:100%;height:300px" />
          </dv-border-box-8>
        </div>
      </div>
</template>

<script>
import capsuleChart from './capsuleChart.vue'

  export default {
  components: { capsuleChart },
  data(){
    return{
      config1:{
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
              }
            ]
        },
        config2:{
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
              },
              {
                name: '信阳',
                value: 45
              },
              {
                name: '漯河',
                value: 29
              }
            ]
        },
        config3:{
          data: [66],
          shape:'roundRect',
          colors:['#f60','green'],
          waveOpacity:[0.8]
        },
        config4:{
              centerPoint: [0.48, 0.35],
              points: [
                {
                  position: [0.52, 0.235],
                  text: '新乡'
                },
                {
                  position: [0.43, 0.29],
                  text: '焦作'
                },
                {
                  position: [0.59, 0.35],
                  text: '开封'
                },
                {
                  position: [0.53, 0.47],
                  text: '许昌'
                },
                {
                  position: [0.45, 0.54],
                  text: '平顶山'
                },
                {
                  position: [0.36, 0.38],
                  text: '洛阳'
                },
                {
                  position: [0.62, 0.55],
                  text: '周口'
                },
                {
                  position: [0.56, 0.56],
                  text: '漯河'
                },
                {
                  position: [0.37, 0.66],
                  text: '南阳'
                },
                {
                  position: [0.55, 0.81],
                  text: '信阳'
                },
                {
                  position: [0.55, 0.67],
                  text: '驻马店'
                },
                {
                  position: [0.37, 0.29],
                  text: '济源'
                },
                {
                  position: [0.20, 0.36],
                  text: '三门峡'
                },
                {
                  position: [0.76, 0.41],
                  text: '商丘'
                },
                {
                  position: [0.59, 0.18],
                  text: '鹤壁'
                },
                {
                  position: [0.68, 0.17],
                  text: '濮阳'
                },
                {
                  position: [0.59, 0.10],
                  text: '安阳'
                }
              ],
              bgImgUrl: require('../assets/img/map.jpg'),
              centerPointImg: {
                url: require('../assets/img/mapCenterPoint.png')
              },
              pointsImg: {
                url: require('../assets/img/mapPoint.png')
              }
        },
        config5:{
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
      value: 71
    },
    {
      name: '驻马店',
      value: 66
    },
    {
      name: '新乡',
      value: 80
    },
    {
      name: '信阳',
      value: 35
    },
    {
      name: '漯河',
      value: 15
    }
  ],

  showValue: true
        }
    }
  }
  }
</script>

<style lang="less" scoped>

</style>