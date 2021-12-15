<template>
  <v-app>
    <Navbar />

    <v-main>
      <Header />
      <Projects />
    </v-main>
  </v-app>
</template>

<script>
import Navbar from "./components/navbar.vue";
import Header from "./components/header.vue";
import Projects from "./components/Projects.vue";
export default {
  name: "App",

  components: {
    Navbar,
    Header,
    Projects,
  },

  data: () => ({
    //
  }),
};
</script>


<style >
body {
  font-family: Verdana, sans-serif !important;
}

#logo-btn {
  letter-spacing: 5px !important;
  font-family: Verdana, sans-serif !important;
  font-size: 15px;
}
.v-main {
  max-width: 1500px !important;
  margin: 0 auto !important;
  padding: 0 !important;
}
</style>