<template>
    <v-container>
        <div class="card-container">
            <v-card class="image-card">
                <v-img src="../assets/images/mokpo.jpg" :fill-height="true"></v-img>
                <!-- <v-card-title>{{ 관광추천 }}</v-card-title>
                <v-card-text>{{ 추천지1 }}</v-card-text> -->
            </v-card>
            <v-card class="image-card">
                <v-img src="../assets/images/mokpo2.jpg" :fill-height="true"></v-img>
                <!-- <v-card-title>{{ 관광추천 }}</v-card-title> -->
                <!-- <v-card-text>{{ 추천지2 }}</v-card-text> -->
            </v-card>
            <v-card class="image-card">
                <v-img src="../assets/images/logo.png" :fill-height="true"></v-img>
                <!-- <v-card-title>{{ 관광추천 }}</v-card-title> -->
                <!-- <v-card-text>{{ 추천지3 }}</v-card-text> -->
            </v-card>
        </div>
    </v-container>
</template>

<script>
</script>

<style>
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
</style>