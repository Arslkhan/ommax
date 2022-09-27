<template>
  <div id="app">
    <Header></Header>
    <router-view />
    <Footer></Footer>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
export default {
  name: 'App',
  components: {
    Header,
    Footer
  }
};
</script>
<style lang="scss">
  #app {
    // font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }
  @font-face {
  font-family: "IBMPlexRegular";
  src: url(./fonts/IBMPlexSans-Regular.ttf) format("truetype");
  }
  @font-face {
    font-family: "IBMPlexBold";
    src: url(./fonts/IBMPlexSans-Bold.ttf) format("truetype");
  }
  body {
    font-family: "IBMPlexRegular", sans-serif;
    overflow-x: hidden;
  }
  .default-btn {
      background: rgb(1, 164, 183) !important;
      border-radius: 5px !important;
      color: #fff !important;
      padding: 12px 10px !important;
      width: 9.375rem;
      font-family: "IBMPlexBold", sans-serif !important;
      transform: scale( 1 );
      transition: 0.15s all ease;

      &:hover,
      &:focus {
        background: rgb(0, 126, 145) !important;
        color: #fff !important;
        transform: scale(1.06);
      }
    }
</style>
