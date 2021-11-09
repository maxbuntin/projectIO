<template>
  <div class="text-center">
    <h1>Переваги</h1>

    <v-container class="grey lighten-5">
      <v-row>
        <v-col>
          <v-card class="d-flex justify-center align-center" height="370">
            <div>
              <img src="../assets/Group 11.png" />
              <v-card-text
                >Легкий перегляд пов’язаної інформації у одному
                місці</v-card-text
              >
            </div>
          </v-card>
        </v-col>
        <v-col>
          <v-card class="d-flex justify-center align-center" height="370">
            <div>
              <img src="../assets/Group 17.png" />
              <v-card-text
                >Простий інтерфейс у стилі material design</v-card-text
              >
            </div>
          </v-card>
        </v-col>

        <v-col>
          <v-card class="d-flex justify-center align-center" height="370">
            <div>
              <img src="../assets/Group 12.png" />
              <v-card-text
                >Швидка авторизація через Google OAuth 2.0</v-card-text
              >
            </div>
          </v-card>
        </v-col>
        <v-col>
          <v-card class="d-flex justify-center align-center" height="370">
            <div>
              <img src="../assets/Group 13.png" />
              <v-card-text
                >Доступ з будь-якого сучасного веб-браузера</v-card-text
              >
            </div>
          </v-card>
        </v-col>
        <v-col>
          <v-card class="d-flex justify-center align-center" height="370">
            <div>
              <img src="../assets/Group 19.png" />
              <v-card-text
                >Інтеграція з Google Workspace</v-card-text
              >
            </div>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "Header",
  data: () => ({}),
};
</script>

<style scoped>

img {
  width: 85px;
  height: 85px;
}

h1 {
  font-family: "Nunito";
  color: #00084d;
  font-size: 48px;
  margin: 50px 0 76px 0;
}
.v-card {
  background: #ffffff;
  box-shadow: 0px 0px 40px 2px rgba(28, 44, 190, 0.3);
  border-radius: 15px;
}

</style>
