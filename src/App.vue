<template>
  <v-app id="inspire">
   <Header />
    <InventorySystem />

    <WorkWithUs />
    <Benefits />
    <Problems />
    <GetAccess />
    <Footer />
    <!-- <v-main>
      <router-view />
    </v-main> -->
  </v-app>
</template>

<script>
 import Header from "./components/Header";
import Footer from "./components/Footer";
import Problems from "./components/Problems";
 import Benefits from "./components/Benefits";
import GetAccess from "./components/GetAccess";
 import InventorySystem from "./components/InventorySystem";
import WorkWithUs from "./components/WorkWithUs";

export default {
  name: "App",
  components: {
   Header,
   InventorySystem,
    Problems,
    Footer,
   Benefits,
    GetAccess,
    WorkWithUs,
  },
  data() {
    return {
      menu: [
        { icon: "home", title: "Link A" },
        { icon: "info", title: "Link B" },
        { icon: "warning", title: "Link C" },
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

<style>
h1 {
  font-family: "Nunito";
  font-size: 48px;
  color: #00084d;
}

.pa-6 {
  display: none;
}
</style>
