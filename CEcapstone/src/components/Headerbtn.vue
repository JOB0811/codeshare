<template>
  <div class="header">
    <div class="toggle-button" @click="toggleMenu">
      <svg viewBox="0 0 100 80" width="30" height="30">
        <rect width="100" height="10"></rect>
        <rect y="30" width="100" height="10"></rect>
        <rect y="60" width="100" height="10"></rect>
      </svg>
    </div>
    <a class="Hbtn">목포 지역관광</a>
    <nav>
      <ul>
        <li><a>홈</a></li>
        <li><a>지역 소개</a></li>
        <li><a>문의</a></li>
        <li><a @click="openModal">로그인</a>
          <Loginli>
            <form>
              <label for="email">이메일</label>
              <input type="email" id="email" required>

              <label for="password">비밀번호</label>
              <input type="password" id="password" required>

              <button type="submit">로그인</button>
            </form>
          </Loginli>
        </li>
      </ul>
    </nav>
  </div>
</template>
  
<script>
import Loginli from './loginli.vue';

export default {
  data() {
    return {
      menuOpen: false
    };
  },
  methods: {
    toggleMenu() {
      this.menuOpen = !this.menuOpen;
    }
  },
  components: { Loginli}
};
</script>
  
<style>
.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem;
  background-color: #f8f8f8;
  border-bottom: 1px solid #ccc;
}

nav ul {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
}

nav li {
  margin-right: 1rem;
}

nav a {
  background-color: #42a5f5;
  color: #ffffff;
  font-weight: bold;
  border-radius: 20px;
  padding: 8px 16px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
  font-size: 1.1rem;
}

a {
  padding-left: 30px;
}

.Hbtn {
  font-size: 30px;
  font-family: 'Montserrat', sans-serif;
  /* Montserrat 폰트 사용 */
  font-weight: bold;
  color: #333;
  margin-left: 300px;
  /* 원하는 색상으로 변경 */
  text-transform: uppercase;
  letter-spacing: 0.1rem;
  /* margin: 1rem 0; */
}
</style>