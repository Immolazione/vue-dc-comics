<template>
  <div class="page-size">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
  import Header from './components/Header.vue'
  import Main from './components/Main.vue'
  import Footer from './components/Footer.vue'

  export default {
    name: 'App',
    components: {
      Header,
      Main,
      Footer
    }
  }
</script>

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  .page-size {
    height: 100vh;
  }
  .container {
    width: 1200px;
    margin: 0 auto;
  }
</style>
