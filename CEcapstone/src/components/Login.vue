<template>
  <div>
    <v-btn class="button" @click="showModal = true">로그인</v-btn>
    <v-dialog v-model="showModal" max-width="500" class="dialog">
      <v-card>
        <v-img src="https://www.mokpo.go.kr/build/images/1517/15173024/1517302477.jpg/666x1x85/666x1_1517302477.jpg"
          height="200" cover></v-img>
        <v-card-title class="title">목포 지역관광</v-card-title>
        <v-card-title>
          <span class="headline">로그인</span>
        </v-card-title>
        <v-card-text>
          <v-text-field label="아이디" outlined style="background-color: #fffff; border-radius: 4px;"
            v-model="username"></v-text-field>
          <v-text-field label="비밀번호" outlined style="background-color: #fffff; border-radius: 4px;" v-model="password"
            type="password"></v-text-field>
        </v-card-text>
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn color="#fffff" text @click="showModal = false">취소</v-btn>
          <v-btn color="#fffff" text @click="login">로그인</v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
    <div class="modal">
      <div class="modal__overlay"></div>
      <div class="modal__body">
        <!-- 모달창 내용 -->
      </div>
    </div>
  </div>
</template>
  
<script>
export default {
  data() {
    return {
      showModal: false,
      username: '',
      password: ''
    }
  },
  methods: {
    login() {
      // 로그인 처리 로직
      console.log(`username: ${this.username}, password: ${this.password}`)
      this.showModal = false
    }
  }
}
</script>


<style>
.button {
  background-color: #42a5f5;
  color: #ffffff;
  font-weight: bold;
  border-radius: 20px;
  padding: 8px 16px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
  font-size: 1.1rem;
  text-align: right;
  position: absolute;
  top: 0;
  right: 0;
  /* margin-top: 110px; */
  margin-right: 300px;

}

.title {
  text-align: center;
}


.button:hover {
  background-color: #333;
  color: white;
}

/* .fixed-header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  background-color: #fff;
} */
</style>