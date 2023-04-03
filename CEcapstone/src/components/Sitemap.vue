<template>
    <v-container>
      <v-row>
        <v-col v-for="(button, index) in buttons" :key="index" cols="12">
          <v-btn :color="button.color">{{ button.text }}</v-btn>
        </v-col>
      </v-row>
    </v-container>
  </template>
  
  <script>
  export default {
    data() {
      return {
        buttons: [
          { text: '문의', color: '' },
          { text: '이메일 기입', color: '' },
          { text: '전화번호 기입', color: '' },
        ]
      }
    }
  }
  </script>
<style>
</style>