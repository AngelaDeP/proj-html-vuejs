<template>
    <div class="columns-pd-container">
        <div class="column-content">
            <h3>FEATURED</h3>
                <div class="style-column" v-for="(feature, index) in featured" :key="index">
                    <div class="style-text">
                        <div class="product-name">{{feature.product}}</div>
                        <div class="prices">
                            <span class="discounted-price">{{feature.discountedPrice}}</span>
                            <span class="price">{{feature.price}}</span>
                        </div>
                    </div>
                    <div class="style-image">
                        <img :src="require(`../assets/img/` + feature.url)">
                    </div>
                </div>
        </div>
        <div class="column-content">
            <h3>ON SALE</h3>
                <div class="style-column" v-for="(sale, index) in onSale" :key="index">
                    <div class="style-text">
                        <div class="product-name">{{sale.product}}</div>
                        <div class="prices">
                            <span class="discounted-price">{{sale.discountedPrice}}</span>
                            <span class="price">{{sale.price}}</span>
                        </div>
                    </div>
                    <div class="style-image">
                        <img :src="require(`../assets/img/` + sale.url)">
                    </div>
                </div>
        </div>
        <div class="column-content">
            <h3>TOP RATED</h3>
                <div class="style-column" v-for="(rated, index) in topRated" :key="index">
                    <div class="style-text">
                        <div class="product-name">{{rated.product}}</div>
                        <div class="prices">
                            <span class="discounted-price">{{rated.discountedPrice}}</span>
                            <span class="price">{{rated.price}}</span>
                        </div>
                    </div>
                    <div class="style-image">
                        <img :src="require(`../assets/img/` + rated.url)">
                    </div>
                </div>
        </div>    
        <div class="column-content">
            <h3>LATEST REVIEWS</h3>
                <div class="style-column" v-for="(review, index) in latestReviews" :key="index">
                    <div class="style-text">
                        <div class="product-name">{{review.product}}</div>
                        <div class="prices">
                            <span class="discounted-price">{{review.discountedPrice}}</span>
                            <span class="made-by">by {{review.madeBy}}</span>
                        </div>
                    </div>
                    <div class="style-image">
                        <img :src="require(`../assets/img/` + review.url)">
                    </div>
                </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ColumnProducts',
    data() {
    return {
      featured: [
          {
              url: 'black_leather_jacket-120x156.jpg',
              product: "Black Jacket",
              ratings: "",
              price: "$125"
          },
          {
              url: 'black_elegant_leather_jacket-120x156.jpg',
              product: "Black Leather Jacket",
              ratings: "5",
              price: "$200",
              discountedPrice: "$235"
          },
          {
              url: 'hipster_black_top-120x156.jpg',
              product: "Hipster Black Tee",
              ratings: "",
              price: "$57"
          },
      ],
      onSale: [
          {
              url: 'black_elegant_leather_jacket-120x156.jpg',
              product: "Black Leather Jacket",
              ratings: "5",
              price: "$200",
              discountedPrice: "$235"
          },
          {
              url: 'blue_leather_jacket-120x156.jpg',
              product: "Blue Leather Jacket",
              ratings: "5",
              price: "$60",
              discountedPrice: "$80"
          },
          {
              url: 'modern_leather_boots-120x156.jpg',
              product: "Modern Leather Boots",
              ratings: "",
              price: "$30",
              discountedPrice: "$50"
          },
      ],
      topRated: [
          {
              url: 'leather_gloves-120x156.jpg',
              product: "Leather Gloves",
              ratings: "",
              price: "$45"
          },
          {
              url: 'black_elegant_leather_jacket-120x156.jpg',
              product: "Black Leather Jacket",
              ratings: "5",
              price: "$200",
              discountedPrice: "$235"
          },
          {
              url: 'spring_printed_dress-120x156.jpg',
              product: "Spring Printed Dress",
              ratings: "",
              price: "$47"
          },
      ],
      latestReviews: [
          {
              url: 'leather_gloves-120x156.jpg',
              product: "Leather Gloves",
              ratings: "",
              madeBy: "admin"
          },
          {
              url: 'black_elegant_leather_jacket-120x156.jpg',
              product: "Black Leather Jacket",
              ratings: "5",
              price: "$200",
              madeBy: "Beardman"
          },
          {
              url: 'spring_printed_dress-120x156.jpg',
              product: "Spring Printed Dress",
              ratings: "",
              madeBy: "admin"
          },
      ],
    }
  }
}
</script>

<style scoped>
@import "../assets/style/column-products.scss";
</style>