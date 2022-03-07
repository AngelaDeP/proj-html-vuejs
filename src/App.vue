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
    <BrandLogos />
    <SubscribeOffer />
    <MyFooter v-bind:infos="infos" />
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
import BrandLogos from './components/BrandLogos.vue'
import SubscribeOffer from './components/SubscribeOffer.vue'
import MyFooter from './components/MyFooter.vue'

export default {
  name: 'App',
  data() {
    return {
      infos: 
       {
          street: '12345 North Main Street',
          city: 'New York, NY 555555', 
          phone: '1.800.555.6789'},
          email: 'info@company.com',
          web: 'Theme-fusion@com'

        }
    },
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
      ColumnProducts,
      BrandLogos,
      SubscribeOffer,
      MyFooter
    }
}
</script>

<style lang="scss">
@import "./assets/style/general.scss";
@import '~@fortawesome/fontawesome-free/css/all.css'
</style>
