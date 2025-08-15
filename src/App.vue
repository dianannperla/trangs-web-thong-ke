<template>
  <v-app>
    <v-container>
      <h1>Trang Web Thống Kê</h1>
      <data-input></data-input>
      <data-chart></data-chart>
    </v-container>
  </v-app>
</template>

<script>
import DataInput from './components/DataInput.vue';
import DataChart from './components/DataChart.vue';

export default {
  components: {
    DataInput,
    DataChart
  }
}
</script>

<style>
</style>
