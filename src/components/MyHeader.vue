<template>
    <div class="sec-header">
        <div class="header-top">
            <div class="social-sec">
                <ul class="social-list">
                    <li>
                        <a href="#">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="fab fa-twitter"></i>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="fab fa-instagram"></i>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="fab fa-youtube"></i>
                        </a>
                    </li>
                </ul>
            </div>
            <div class="account-sec">
                <ul class="account-list">
                    <li>
                        <a href="#">
                            Shopping Cart
                        </a>
                    </li>
                    <li class="account-element">
                        <a href="#">
                            My Account
                            <i class="fa-solid fa-angle-down"></i>
                        </a>
                    </li>
                    <li class="cart-element">
                        <a href="#">
                            CART
                        </a>    
                    </li>
                </ul>
            </div>
        </div>
        <div class="header-bottom">
            <div class="logo-sec">
                <img src="../assets/img/classic_shop_logo1x.png" alt="">
            </div>
            <div class="right-header-sec">
                <nav>
                    <ul>
                        <li v-for="(link, index) in links" :key="index">
                            <a :href="link.url">{{link.text}}</a>
                            <i class="fa-solid fa-angle-down"></i>
                        </li>
                    </ul>
                </nav>
                <button class="shop-now">SHOP NOW!</button>
                <span class="search-icon">
                    <a href="#">
                        <i class="fa-solid fa-magnifying-glass"></i>
                    </a>
                </span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MyHeader',
    data() {
    return {
      links: [
          {
              text: "Home",
              url: "#",
          },
          {
              text: "Shop",
              url: "#",
          },
          {
              text: "Products",
              url: "#",
          },
          {
              text: "Categories",
              url: "#",
          },
          {
              text: "News",
              url: "#",
          },
          {
              text: "Elements",
              url: "#",
          },
      ],
    }
  }
}
</script>

<style scoped>
@import "../assets/style/myheader.scss";
</style>