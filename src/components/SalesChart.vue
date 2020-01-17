<template lang="pug">
  .sales-chart-contaienr
    HighchartsVue( :options="options" ref="highcharts" )

</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'
import HighchartsVue from 'highcharts-vue'
import {Chart} from 'highcharts-vue'


@Component({
  components: {
    HighchartsVue: Chart 
  }
})
export default class SalesChart extends Vue {
  
options = {
  title: {
    text: 'Monthly Average Sales',
    x: -20, //center
    style: {
      color: "#56657F"
    }
  },
  credits: {
    enabled: false
  },
  chart: {
     backgroundColor: '#212936',
     polar: true,
     type: 'line',
  },
  subtitle: {
    text: 'Source: WorldClassSales.com',
    x: -20,
    style: {
      color: "#56657F"
    }
  },
  xAxis: {
    lineColor: '#8997B1',
    categories: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun',
      'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec'
    ],
     crosshair: {
      color: '#AAAAAA22',
    },
  },
  yAxis: {
    title: {
      text: 'Sales (%)'
    },
    plotLines: [{
      value: 0,
      width: 1,
    }],
      gridLineColor: '#8997B1',

  },
  tooltip: {
    valueSuffix: '°C'
  },
  legend: {
    itemStyle: {
      color: '#8997B1'
    },
    itemHoverStyle: {
      color: '#767988',
    },
    layout: 'vertical',
    align: 'right',
    verticalAlign: 'middle',
    borderWidth: 0,
  },
  series: [{
    name: 'Product-1',
    data: [7.0, 6.9, 9.5, 14.5, 18.2, 21.5, 25.2, 26.5, 23.3, 18.3, 13.9, 9.6]
  }, {
    name: 'Product-2',
    data: [-0.2, 0.8, 5.7, 11.3, 17.0, 22.0, 24.8, 24.1, 20.1, 14.1, 8.6, 2.5]
  }, {
    name: 'Product-3',
    data: [-0.9, 0.6, 3.5, 8.4, 13.5, 17.0, 18.6, 17.9, 14.3, 9.0, 3.9, 1.0]
  }, {
    name: 'Product-4',
    data: [3.9, 4.2, 5.7, 8.5, 11.9, 15.2, 17.0, 16.6, 14.2, 10.3, 6.6, 4.8]
  }]
};
  
}

</script>

<style lang="sass">
.sales-chart-contaienr
  margin-left: 265px
  margin-top: 12px
  width: 750px
  padding: 10px
  height: 434px
  border-radius: 5px
  background-color: #212936
  border: 1px solid #313C4E
  box-shadow: 0px 6px 10px rgba(0, 0, 0, 0.14), 0px 1px 18px rgba(0, 0, 0, 0.12), 0px 3px 5px rgba(0, 0, 0, 0.2)


</style>