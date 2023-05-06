<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'
import IconComp from './components/IconComp.vue'
import FooterComp from './components/FooterComp.vue'
import FumettiComp from './components/FumettiComp.vue';
export default {
  name: "app",
  components: {
    HeaderComp,
    MainComp,
    IconComp,
    FooterComp,
    FumettiComp
  }
}
</script>

<template>
  <!-- NAVBAR -->
  <HeaderComp />

  <main>
    <!-- CONTENT -->
    <MainComp />
    <!-- MERCHANDISE -->
    <IconComp />
  </main>

  <FooterComp />
</template>

<style lang="scss">
@use './style/main.scss' as *;
</style>
