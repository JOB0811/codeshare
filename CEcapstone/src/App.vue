<template>
  <v-app>
    <v-main>
      <div class="background-image">
    <Headerbtn/>
          <h1 class = "letter-spacing">목포에 오신 것을 환영합니다!</h1>
          <p class = "letter-spacing">Welcome to visit Mokpo</p>
          <a></a><br>
          <a></a><br>
          <a href="#">
          <img src="https://blog.kakaocdn.net/dn/uqJpZ/btqyenBIIXx/mh1Cc5F023UGpfQTFBdqV0/img.jpg" class="app-store-button" alt="Download on the App Store" />
          </a>
          <a href="#">
          <img src="https://blog.kakaocdn.net/dn/bDTFBH/btqOhuf3oId/FMaicByKnbnp0lGXSzfJQ0/img.png" class="play-store-button" alt="Download on the play Store" />
          </a>
          <v-container>
      <div class="card-container">
        <v-card class="image-card">
          <v-card-media
            :src="('@/image/Mokpo.jpg')"
            height="200px"
          />
          <v-card-title>{{ 관광추천 }}</v-card-title>
          <v-card-text>{{ 추천지1 }}</v-card-text>
        </v-card>
        <v-card class="image-card">
          <v-card-media
            :src="imageSrc2"
            height="200px"
          />
          <v-card-title>{{ 관광추천 }}</v-card-title>
          <v-card-text>{{ 추천지2 }}</v-card-text>
        </v-card>
        <v-card class="image-card">
          <v-card-media
            :src="imageSrc3"
            height="200px"
          />
          <v-card-title>{{ 관광추천 }}</v-card-title>
          <v-card-text>{{ 추천지3 }}</v-card-text>
        </v-card>
      </div>
    </v-container>
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
        <Componentemail/>
      </v-col>
      <v-col cols="4"></v-col>
      <v-col cols="4" class="alighn-end mt-20">
        <Componentsubscribe/>

      </v-col>
    </v-row>
  </v-container>

<v-divider :thickness="3" color="success"></v-divider>
      <v-container >
      <v-row>
        <v-col cols="3">
          <Sitemap/>
        </v-col>
        <v-col cols="3">
        <Sitemenu/>
        </v-col>
        <v-col cols="3">
        <Sitesns/>
        </v-col>
        <v-col cols="3">
        <Sitedownload/>
        </v-col>
    </v-row>
  </v-container>
      <Footer/>
    </v-main>
  </v-app>
</template>

<script>
import Headerbtn from './components/Headerbtn.vue';
// import Appbar from './components/Appbar.vue'
import Componentemail from './components/Componentemail.vue'
import Footer from './components/Footer.vue'
import Sitemap from './components/Sitemap.vue';
import Sitesns from './components/Sitesns.vue'
import Sitemenu from './components/Sitemenu.vue';
import Sitedownload from './components/Sitedownload.vue'
import Componentsubscribe from './components/Componentsubscribe.vue'

export default {
  name: 'App',

  components: {
    Headerbtn,
    // Appbar,
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
    letter-spacing: 0.2em; 
    margin-left: 50px;
    padding-top: 40px;
  }
.app-store-button {
  width: 80px;
  height: 80px;
  position: relative;
  top: 20px;
  left: 5%;
  right: 50%;
  bottom: 25%;
  transform: translate(-50%, -50%);
  border-radius: 25px;
}

.play-store-button {
  width: 150px;
  height: 75px;
  position: relative;
  top: 15px;
  left: 8%;
  right: 40%;
  bottom: 20px;
  transform: translate(-50%, -50%);
  border-radius: 25px;
}


.card-container {
  display: flex;
  justify-content: space-between;
}

.image-card {
  flex: 1;
  margin-right: 40px;
  background: rgba(255, 255, 255, 0.7);
  padding : 80px;
  margin-top: 12em;
}

.image-card:last-child {
  margin-right: 0;
}


.component-main{
  background-image: url('https://www.socialfocus.co.kr/news/photo/201910/5296_7612_5032.jpg');
  background-repeat: no-repeat;
  background-size: cover;
}
</style>