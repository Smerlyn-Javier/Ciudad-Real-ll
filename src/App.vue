<template>
  <div id="app">
    <!-- <sidebar></sidebar>
    <slider></slider>-->
    <Release></Release>
    <Footer class="footer"></Footer>
  </div>
</template>

<script>
import Sidebar from "../src/components/layouts/sidebar";
import Slider from "../src/components/slider";
import Release from "../src/components/release-card";
import Footer from "../src/components/layouts/footer";
export default {
  name: "app",
  components: {
    Sidebar,
    Footer,
    Slider,
    Release
  }
};
</script>

<style>
* {
  margin: 0px;
  padding: 0px;
}
.footer {
  position: relative;
  margin-top: 40%;
}
</style>
