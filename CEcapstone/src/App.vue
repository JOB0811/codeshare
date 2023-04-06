<template>
  <v-app>
    <v-main>
      <div class="background-image">
        <Headerbtn/>
        <!-- <Login /> -->
        <h1 class="letter-spacing">목포에 오신 것을 환영합니다!</h1>
        <h2 class="letter-spacing2">WELCOME TO VISIT MOKPO</h2>
        <a></a><br>
        <a></a><br>
        <a href="#">
          <img src="https://blog.kakaocdn.net/dn/uqJpZ/btqyenBIIXx/mh1Cc5F023UGpfQTFBdqV0/img.jpg"
            class="app-store-button" alt="Download on the App Store" />
        </a>
        <a href="#">
          <img src="https://blog.kakaocdn.net/dn/bDTFBH/btqOhuf3oId/FMaicByKnbnp0lGXSzfJQ0/img.png"
            class="play-store-button" alt="Download on the play Store" />
        </a>
        <imagecard/>
        <a></a><br>
        <a></a><br>
        <a></a><br>
        <a></a><br>
        <a></a><br>
        <a></a><br>
        <a></a><br>
        <a></a><br>
        <a></a><br>
        <a></a><br>
        <a></a><br>
        <a></a><br>
      </div>
      <!-- <Appbar/> -->
      <v-container class="Component-main" fluid>
        <v-row>
          <v-col cols="4">
            <Componentemail></Componentemail>
          </v-col>
          <v-col cols="4"></v-col>
          <v-col cols="4" class="alighn-end mt-20">
            <Componentsubscribe />

          </v-col>
        </v-row>
      </v-container>

      <v-divider :thickness="3" color="success"></v-divider>
      <v-container>
        <v-row>
          <v-col cols="3">
            <Sitemap />
          </v-col>
          <v-col cols="3">
            <Sitemenu />
          </v-col>
          <v-col cols="3">
            <Sitesns />
          </v-col>
          <v-col cols="3">
            <Sitedownload />
          </v-col>
        </v-row>
      </v-container>
      <Footer></Footer>
    </v-main>
  </v-app>
</template>

<script>
// import Login from './components/Login.vue';
import Headerbtn from './components/Headerbtn.vue';
import imagecard from './components/imagecard.vue';
import Componentemail from './components/Componentemail.vue';
import Footer from './components/Footer.vue';
import Sitemap from './components/Sitemap.vue';
import Sitesns from './components/Sitesns.vue';
import Sitemenu from './components/Sitemenu.vue';
import Sitedownload from './components/Sitedownload.vue';
import Componentsubscribe from './components/Componentsubscribe.vue';

export default {
  name: 'App',

  components: {
    // Login,
    Headerbtn,
    imagecard,
    Componentemail,
    Componentsubscribe,
    Sitemap,
    Footer,
    Sitesns,
    Sitemenu,
    Sitedownload
  },

  data: () => ({
    //
  }),
}
</script>
<style>
.background-image {
  background-image: url('https://www.mokpo.go.kr/build/images/1517/15173024/1517302477.jpg/666x1x85/666x1_1517302477.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  min-height: 300px;
}



.letter-spacing {
  letter-spacing: 0.1em;
  text-align: center;
  margin-top: 20px;
  padding-top: 40px;
  padding: 50px;
  border-radius: 10px;
  color: #333333;
  /* font-style: italic; */
  font-size: 50px;
  font-weight: bold;
  text-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}

.letter-spacing2 {
  letter-spacing: 0.1em;
  text-align: center;
  margin-top: 20px;
  padding-top: 40px;
  padding: 50px;
  border-radius: 10px;
  color: #333333;
  /* font-style: italic; */
  font-size: 30px;
  font-weight: bold;
  text-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}

.app-store-button {
  width: 80px;
  height: 80px;
  position: relative;
  text-align: center;
  margin-left: 600px;
  transform: translate(-50%, -50%);
  border-radius: 50px;
}

.play-store-button {
  width: 200px;
  height: 75px;
  position: relative;
  top: 15px;
  left: 8%;
  right: 40%;
  bottom: 40px;
  margin-bottom: 20px;
  transform: translate(-50%, -50%);
  border-radius: 50px;
}


.card-container {
  display: flex;
  justify-content: space-between;
}

.image-card {
  flex: 1;
  margin-right: 60px;
  background: rgba(255, 255, 255, 0.7);
  margin-top: 12em;
}

.image-card:last-child {
  margin-right: 0;
}


.component-main {
  background-image: url('https://www.socialfocus.co.kr/news/photo/201910/5296_7612_5032.jpg');
  background-repeat: no-repeat;
  background-size: cover;
}
</style>