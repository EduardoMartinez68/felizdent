<template>
  <div id="app">
    <Header /> <!-- Header  -->
    <router-view></router-view> <!-- Contenido de la página -->
    <LlamadaButton />
    <WhatsAppButton />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import WhatsAppButton from './components/WhatsAppButton.vue';
import LlamadaButton from './components/LlamadaButton.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    WhatsAppButton,
    LlamadaButton,
    Footer
  },
}
</script>

<style>

</style>
