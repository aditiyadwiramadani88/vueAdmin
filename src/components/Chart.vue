<template>
    <Bar
      id="my-chart-id"
      :options="chartOptions"
      :data="chartData"
    />
  </template>
  
  <script>
  import { Bar } from 'vue-chartjs'
  import { Chart as ChartJS, Title, Tooltip, Legend, BarElement, CategoryScale, LinearScale } from 'chart.js'
  
  ChartJS.register(Title, Tooltip, Legend, BarElement, CategoryScale, LinearScale)
  
  export default {
    components: { Bar },
    data() {
      return {
        chartData: {
          labels: [ 'January', 'February', 'March', 'april', 'jun', 'jul', 'Ags', 'Sep', 'Okt', 'Desc' ],
          datasets: [ { data: [40, 20, 12, 40,20,40, 40 , 12, 18, 20] } ]
        },
        chartOptions: {
          responsive: true, 
          backgroundColor: "lightblue"
        }
      }
    }
  }
  </script>