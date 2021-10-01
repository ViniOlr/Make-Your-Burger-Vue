<template>
  <NavBar :logo="logo_src" :alt="app_name" :v-if="permissão" />
  <router-view/>
  <Footer />
</template>

<script>
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';

export default {
  components: {
    NavBar,
    Footer
  },
  data(){
    return {
      logo_src: '/img/logo.png',
      app_name: "Make your burguer",
      permissão: false
    }
  }
}
</script>

<style>
:root {
  --font: #fcba03;
  --background: #222;
  --border: #111;
}
* {
  font-family: Helvetica, sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 2%;
}
h1.title {
  text-align: center;
  font-size: 2.9em;
  margin: 30px 0;
  color: #222;
}
</style>
