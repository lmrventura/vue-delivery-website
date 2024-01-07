<template>
  <div class="div">
    <Navbar :logo="logo_src" :alt="app_name" />
    <div>
      <router-view/>
    </div>
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';

export default {
  data() {
    return {
      logo_src: "/img/logo.png",
      app_name: "Make your Burger"
    }
  },
  components: {
    Navbar,
    Footer
  }
}
</script>

<style>
  * {
    font-family: Arial, Helvetica, sans-serif;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }
</style>
