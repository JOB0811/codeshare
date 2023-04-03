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
          { text: '사이트 메뉴', color: '' },
          { text: '소개', color: '' },
          { text: '문의', color: '' },
          { text: '개인정보 취급 방침', color: '' },
          { text: '이용약관', color: '' },
        ]
      }
    }
  }
  </script>
<style>
</style>