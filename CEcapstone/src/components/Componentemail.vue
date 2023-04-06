
<!-- 그리드 크기
    xs = 2px
    sm = 4px
    md = 8px
    lg = 16px
    xl = 24px -->


<template>
  <v-card class="mx-auto" max-width="400" title="문의하기">
    <v-container>
      <v-row>
        <v-col cols="6">
          <v-text-field v-model="first" color="primary" label="성" variant="underlined"></v-text-field>
        </v-col>
        <v-col cols="6">
          <v-text-field v-model="last" color="primary" label="이름" variant="underlined"></v-text-field>
        </v-col>
      </v-row>
      <v-text-field v-model="email" color="primary" label="Email" variant="underlined"></v-text-field>

      <v-textarea counter label="저희에게 메시지를 보내주세요!" :rules="rules" :model-value="value"></v-textarea>

    </v-container>

    <v-divider></v-divider>

    <v-card-actions>
      <v-spacer></v-spacer>

      <v-btn color="success">
        완료
      </v-btn>
    </v-card-actions>
  </v-card>
</template>
<script>

</script>


<style></style>