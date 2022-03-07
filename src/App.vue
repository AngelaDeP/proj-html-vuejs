<template>
  <div id="app">
    <MyHeader />
    <MyJumbotron />
    <FeaturedProduct />
    <CollectionSlides />
    <BestSeller />
    <TariffsPrice />
    <NewArrivals />
    <TestimoniesSec />
    <FromOurBlog />
    <hr>
    <ColumnProducts />
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyJumbotron from './components/MyJumbotron.vue'
import FeaturedProduct from './components/FeaturedProduct.vue'
import CollectionSlides from './components/CollectionSlides.vue'
import BestSeller from './components/BestSeller.vue'
import TariffsPrice from './components/TariffsPrice.vue'
import NewArrivals from './components/NewArrivals.vue'
import TestimoniesSec from './components/TestimoniesSec.vue'
import FromOurBlog from './components/FromOurBlog.vue'
import ColumnProducts from './components/ColumnProducts.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    MyJumbotron,
    FeaturedProduct,
    CollectionSlides,
    BestSeller,
    TariffsPrice,
    NewArrivals,
    TestimoniesSec,
    FromOurBlog,
    ColumnProducts
  }
}
</script>

<style lang="scss">
@import "./assets/style/general.scss";
@import '~@fortawesome/fontawesome-free/css/all.css'
</style>
