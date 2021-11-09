<template>
  <v-toolbar>
    <v-toolbar-title> <img src="../assets/footer_logo.png" /></v-toolbar-title>
    <v-spacer></v-spacer>
    <v-toolbar-items class="d-flex align-center">
      <button
        class="btn"
        v-for="item in menu"
        :key="item.title"
        :to="item.link"
      >
        {{ item.title }}
      </button>
      <div class="d-flex align-center">
      <button class="LogIn" @click.stop="dialog = true">Увійти</button>
      </div>

      <v-dialog v-model="dialog">
        <v-card>
          <div class="dialog-content">
            <img src="../assets/footer_logo.png" />

            <div class="head-btn">
              <v-btn class="btn" text @click="dialog = false">
                <v-icon large left> mdi-google-plus </v-icon>
                Google
              </v-btn>

              <v-btn class="btn ml-8" text @click="dialog = false">
                <v-icon large left> mdi-microsoft-windows </v-icon>
                Microsoft</v-btn
              >
            </div>

            <div class="title">
              <span> або </span>
            </div>
            <div class="input text-center">
              <input type="text" placeholder="Ваша пошта" />
            </div>

            <v-btn class="sigin" text @click="dialog = false"> Увійти </v-btn>

            <div class="dialog-footer">Всі права захищено © IO 2021</div>
          </div>
        </v-card>
      </v-dialog>
    </v-toolbar-items>
    <v-menu class="hidden-md-and-up">
      <v-toolbar-side-icon slot="activator"></v-toolbar-side-icon>
      <v-list>
        <v-list-tile v-for="item in menu" :key="item.icon">
          <v-list-tile-content>
            <v-list-tile-title>{{ item.title }}</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-menu>
  </v-toolbar>
</template>

<script>
export default {
name: "InventorySystem",
  data() {
    return {
    dialog: false,
      menu: [
        { title: "Робота з нами" },
        { title: "Проблеми" },
        { title: "Переваги" },
        { title: "Команда" },
      ],
    };
  },

  methods: {
    menuItems() {
      return this.menu;
    },
  },
};
</script>

<style scoped>
.main {
  font-family: "Nunito";
  width: 100%;

  background-color: #d9dcf580;
  height: 800px;
}
.content {
  margin-left: 236px;
  max-width: 830px;
}

button {
  font-family: Nunito;
  font-style: normal;
  font-weight: normal;
  display: justify;
  text-transform: uppercase;
  text-align: center;
  font-size: 18px;
  width: 180px;
  height: 40px;


    margin: 15px 0 15px 0px;
}
.LogIn {
  background: #7683f7;
  border-radius: 15px;
  color: white;
  text-align: center;
  margin: 0 150px 0 0px;
}

.v-toolbar img {
text-align: center;
  width: 161px;
  margin: 15px 0 15px 236px;
  padding:  10px;
  background: none;
}

.v-dialog {
  overflow-y: hidden;
}
.dialog-content {
  background: rgba(255, 255, 255, 0.3);
  border-radius: 15px;
}

.v-card {
  background: linear-gradient(282.65deg, #7683f7 0%, #dde0ff 99.33%);
  backdrop-filter: blur(50px);
  border-radius: 15px;
  justify-content: center;
  text-align: center;
}

.sigin {
  width: 220px;
  height: 50px;
  background: #7683f7;
  border-radius: 10px;
  color: white;
  margin: 50px 0 128px 0;
}

.dialog-content .btn {
  width: 250px;
  height: 20px;
  background: none;
  border: 3px solid #484bf2;
  border-radius: 15px;
  padding: 15px;
}
.head-btn {
  margin-bottom: 60px;
}
.dialog-content img {
  margin-bottom: 85px;
  margin-top: 32px;
  width: 300px;
}

.btn .v-icon {
  color: #484bf2;
  margin-right: 20px;
}

.btn:hover .v-icon {
  color: #ff725e;
}

.btn:hover {
  border: 3px solid #ff725e;
}

.title {
  overflow: hidden;

  text-align: center;
  /* Тут можно добавить другие стили для заголовка */
  font-size: 18px;
  margin-bottom: 95px;
}
.title span {
  font-family: Nunito;
  color: #484bf2;

  display: inline-block;
  vertical-align: middle;
}
.title:before,
.title:after {
  content: "";

  display: inline-block;
  vertical-align: middle;

  width: 344px;
  height: 1px;

  background-color: #484bf2;

  position: relative;
}
.title:before {
  margin-left: -100%;

  left: -14px;
}
.title:after {
  margin-right: -100%;

  right: -14px;
}

.v-text-field {
  text-align: center;
  width: 600px;
}

input {
  width: 550px;
  height: 60px;
  border: 3px solid #7683f7;
  border-radius: 15px;
  padding: 15px;
}

input:hover {
  border: 3px solid #ff725e;
}

.dialog-footer {
  padding: 20px 0;
}
.image {
  margin-left: -300px;
}
</style>
