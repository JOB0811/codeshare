<template>
  <v-divider :thickness="3" color="success"></v-divider>
  <v-footer class="d-flex flex-column">
    <div class="bg d-flex w-100 align-center px-10">

      <v-spacer></v-spacer>

      <strong>목포에서 즐거운 여행을 보내세요!</strong>

      <v-spacer></v-spacer>

      <v-btn v-for="icon in icons" :key="icon" class="mx-4" :icon="icon" variant="plain" size="small"></v-btn>
    </div>

    <div class="px-4 py-2 bg text-center w-100">
      <strong>캡스톤 디자인</strong>
    </div>
  </v-footer>
</template>
<script>
export default {
  data: () => ({
    icons: [
      'mdi-facebook',
      'mdi-twitter',
      'mdi-linkedin',
      'mdi-instagram',
    ],
  }),
}
</script>
<style></style>