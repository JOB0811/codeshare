<template>
  <v-container>
    <v-row align="center">
      <v-col cols="9">
        <v-textarea v-model="text" label="email을 입력해주세요"></v-textarea>
      </v-col>
      <v-col cols="3">
        <v-btn color="primary" @click="submit">Submit</v-btn>
      </v-col>
    </v-row>
  </v-container>
</template>
  
<script>
export default {
  data() {
    return {
      text: '',
    }
  },
  methods: {
    submit() {
      console.log('Submitted text:', this.text);
    },
  },
}
</script>
<style></style>