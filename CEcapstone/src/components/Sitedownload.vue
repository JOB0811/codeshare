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
          { text: '애플', color: '' },
          { text: '안드로이드', color: '' },
        ]
      }
    }
  }
  </script>
<style>
</style>