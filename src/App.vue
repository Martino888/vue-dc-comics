<template>
  <div id="app">
    <HeaderDc />
    <MainDc />
    <FooterMain />
  </div>
</template>

<script>
import HeaderDc from './components/HeaderDc.vue'
import MainDc from './components/MainDc.vue'
import FooterMain from './components/FooterMain.vue'
export default {
  name: 'App',
  components: {
    HeaderDc,
    MainDc,
    FooterMain
  }
}
</script>

<style lang="scss">
#app {
body {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
}
</style>
