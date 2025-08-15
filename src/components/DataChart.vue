<template>
  <v-card>
    <v-card-title>Biểu Đồ</v-card-title>
    <v-card-text>
      <canvas id="myChart"></canvas>
    </v-card-text>
  </v-card>
</template>

<script>
import { Line } from 'chart.js';
export default {
  mounted() {
    const ctx = document.getElementById('myChart').getContext('2d');
    new Line(ctx, {
      type: 'line',
      data: {
        labels: ["Jan", "Feb", "Mar", "Apr"],
        datasets: [{
          label: 'Dữ liệu',
          data: [65, 59, 80, 81],
          borderColor: 'rgba(75, 192, 192, 1)',
          backgroundColor: 'rgba(75, 192, 192, 0.2)',
        }]
      }
    });
  }
};
</script>

<style scoped>
</style>
