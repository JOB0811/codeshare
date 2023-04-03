<template>
  <v-app>
    <v-main>
      <Appbar/>
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
import Appbar from './components/Appbar.vue'
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
    Appbar,
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
.component-main{
  background-image: url('https://www.socialfocus.co.kr/news/photo/201910/5296_7612_5032.jpg');
  background-repeat: no-repeat;
  background-size: cover;
}
</style>