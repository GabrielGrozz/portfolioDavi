<template>
  <div class="main-app">
    <Header class="header d-flex justify-content-center" />
    <Main class="main"/>
    <Footer />
  </div>
  
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue"

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer
  },
};
</script>

<style scoped>
.header {
  height: 100vh;
  flex-direction: column;
}
.main-app{
  background: rgba(255, 255, 255);
}
.main{
  border: rgba(0, 0, 0, 0.5) solid 3px;
  border-bottom: 0;
}


@media screen and (max-width: 615px) {
  .main{
    border: 0;
  }
  }
</style>