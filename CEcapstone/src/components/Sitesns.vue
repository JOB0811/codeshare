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
          { text: '디스코드', color: '' },
          { text: '트위치', color: '' },
          { text: '페이스북', color: '' },
          { text: '유튜브', color: '' },
          { text: '트위터', color: '' },
        ]
      }
    }
  }
  </script>
<style>
</style>