<template>
  <div id="app">
    <MyHeader />
    <MyJumbotron />
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyJumbotron from './components/MyJumbotron.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyJumbotron
  }
}
</script>

<style lang="scss">
@import "./assets/style/general.scss";
@import '~@fortawesome/fontawesome-free/css/all.css'
</style>
