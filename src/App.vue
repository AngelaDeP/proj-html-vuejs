<template>
  <div id="app">
    <MyHeader />
    <MyJumbotron />
    <FeaturedProduct />
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyJumbotron from './components/MyJumbotron.vue'
import FeaturedProduct from './components/FeaturedProduct.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyJumbotron,
    FeaturedProduct
  }
}
</script>

<style lang="scss">
@import "./assets/style/general.scss";
@import '~@fortawesome/fontawesome-free/css/all.css'
</style>
