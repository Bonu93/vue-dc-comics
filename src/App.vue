<template>
  <div id="app">

    <!-- header  -->
    <Header />

    <!-- hero  -->
    <Hero />

    <!-- main -->
    <Main />

    <Bluebanner />

    <!-- footer -->
    <Footer />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Header from '@/components/Header.vue';
import Main from '@/components/Main.vue';
import Footer from '@/components/Footer.vue';
import Hero from '@/components/Hero.vue';
import Bluebanner from '@/components/Bluebanner.vue';



export default {
  name: 'App',
  components: {
    Header,
    Main, 
    Footer,
    Hero,
    Bluebanner,
  }
}
</script>

<style lang="scss">
@import '@/styles/global';
@import '@/styles/utilities';
</style>
