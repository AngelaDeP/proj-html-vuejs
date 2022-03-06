<template>
  <div id="app">
    <MyHeader />
    <MyJumbotron />
    <FeaturedProduct />
    <CollectionSlides />
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyJumbotron from './components/MyJumbotron.vue'
import FeaturedProduct from './components/FeaturedProduct.vue'
import CollectionSlides from './components/CollectionSlides.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyJumbotron,
    FeaturedProduct,
    CollectionSlides
  }
}
</script>

<style lang="scss">
@import "./assets/style/general.scss";
@import '~@fortawesome/fontawesome-free/css/all.css'
</style>
