<template>
  <div class="container">
    <!-- start for Topheader  -->
    <Topheader />
    <!-- end for Topheader  -->
    <!-- start for header  -->
    <Header />
    <!-- end for header  -->
    <!-- start for banner  -->
    <Banner />
    <!-- end for banner  -->
    <!-- start for Available  -->
    <Available />
    <!-- end for Available  -->
    <!-- start for versatilead  -->
    <Versatile />
    <!-- end for versatilead  -->
    <!-- start for inspection  -->
    <Inspection />
    <!-- end for inspection  -->
    <!-- start for slider  -->
    <!-- end for slider  -->
    <!-- start for footer  -->
    <Footer />
    <!-- end for footer  -->
  </div>
</template>
<script>
import Topheader from './components/Topheader.vue';
import Header from './components/Header.vue';
import Banner from './components/Banner.vue';
import Available from './components/Available.vue';
import Versatile from './components/Versatilead.vue';
import Footer from './components/Footer.vue';
import Inspection from './components/Inspection.vue';
export default {
  name: 'App',
  components: {
    Topheader,
    Header,
    Banner,
    Available,
    Versatile,
    Inspection,
    Footer
  },
  data() {
    return {

    }
  }
}
</script>
<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=PT+Sans&display=swap');
*,*::before,*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'PT Sans', sans-serif;
}
body{
  background: #F2F2F2;
}
</style>
