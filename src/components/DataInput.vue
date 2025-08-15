<template>
  <v-card>
    <v-card-title>Nhập Dữ Liệu</v-card-title>
    <v-card-text>
      <v-text-field v-model="inputData" label="Nhập dữ liệu"></v-text-field>
      <v-btn @click="addData">Thêm</v-btn>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  data() {
    return {
      inputData: '',
    };
  },
  methods: {
    addData() {
      // Logic để thêm dữ liệu
      this.inputData = '';
    }
  }
};
</script>

<style scoped>
</style>
