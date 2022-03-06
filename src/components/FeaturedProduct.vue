<template>
    <div class="container-ft-products">
        <div class="ft-products-sec">
            <div class="title-ft-products">
                <h2>Featured Products</h2>
            </div>
            <span>Must have products from our top sellers</span>
        </div>
        <div class="nav-ft-products">
            <ul>
                <li>
                    <a href="#">Men</a>
                </li>
                <li>
                    <a href="#">Women</a>
                </li>
                <li>
                    <a href="#">Accessories</a>
                </li>
            </ul>
        </div>
        <div class="ft-products-content">
            <div class="ft-product-card">
                <div class="ft-product-card-img">
                    <img src="../assets/img/black_elegant_leather_jacket.jpg" alt="">
                </div>
                <div class="ft-product-card-text">
                    <h1>Black Leather Jacket</h1>
                    <div class="tags">Men, Jackets, Jeans</div>
                    <br>
                    <span class="original-price">$235</span>
                    <span>$200</span>
                </div> 
            </div>
            <div class="ft-product-card">
                <div class="ft-product-card-img">
                    <img src="../assets/img/black_leather_suit.jpg" alt="">
                </div>
                <div class="ft-product-card-text">
                    <h1>Black Leather Suit</h1>
                    <div class="tags">Men, Jackets</div>
                    <br>
                    <span>$176</span>
                </div> 
            </div>
            <div class="ft-product-card">
                <div class="ft-product-card-img">
                    <img src="../assets/img/blue_jacket_and_white_stripe_tee.jpg" alt="">
                </div>
                <div class="ft-product-card-text">
                    <h1>Blue Jacket & Striped Tee</h1>
                    <div class="tags">Men, Jackets, Suits</div>
                    <br>
                    <span>$580</span>
                </div> 
            </div>
            <div class="ft-product-card">
                <div class="ft-product-card-img">
                    <img src="../assets/img/modern_black_leather_suit.jpg" alt="">
                </div>
                <div class="ft-product-card-text">
                    <h1>Modern Black Leather Suit</h1>
                    <div class="tags">Men, Jackets</div>
                    <br>
                    <span>$96</span>
                </div> 
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FeaturedProduct'
}
</script>

<style scoped>
@import "../assets/style/featuredproduct.scss";
</style>