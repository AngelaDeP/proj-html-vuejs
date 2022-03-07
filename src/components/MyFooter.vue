<template>
<div class="footer-container">
    <div class="top-footer-container">
        <div class="tf-content">
                <div class="personal-info">
                    <img class="cs-logo" src="../assets/img/classic_shop_logo1x.png">
                    <div class="info-text">
                        <div>{{infos.street}}</div>
                        <div>{{infos.city}}</div>
                        <div>Phone: {{infos.phone}}</div>
                        <div>Email: {{infos.email}}</div>
                        <div>Web: {{infos.web}}</div>
                    </div>
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
                </div>
                
                <div class="column-content style-text">
                    <h3>TOP RATED PRODUCTS</h3>
                        <div class="style-column" v-for="(rated, index) in topRated" :key="index">
                            <div class="style-text">
                                <div class="product-name">{{rated.product}}</div>
                                <div class="ratings">
                                    <i v-for="i in 5" :key="i" class="fa-star fa-solid"></i>
                                </div>
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
                <div class="column-content style-text">
                    <h3>RECENT POSTS</h3>
                        <div class="posts-list">
                            <ul>
                                <li>
                                    <i class="fa-solid fa-chevron-right"></i>
                                    <span>Aenean lobortis sapien enim viverra</span>
                                </li>
                                <li>
                                    <i class="fa-solid fa-chevron-right"></i>
                                    <span>Duis ac massa semper maximus</span>
                                </li>
                                <li>
                                    <i class="fa-solid fa-chevron-right"></i>
                                    <span>Nunc fermit nulla eu justo sem id</span>
                                </li>
                                <li>
                                    <i class="fa-solid fa-chevron-right"></i>
                                    <span>Aliquam posuere magna eget nibh</span>
                                </li>
                                <li>
                                    <i class="fa-solid fa-chevron-right"></i>
                                    <span>Cras ac nulla ac consecte rutrum</span>
                                </li>
                                <li>
                                    <i class="fa-solid fa-chevron-right"></i>
                                    <span>Fusce mattis nunc ut aliquam</span>
                                </li>
                            </ul>
                        </div>
                </div>
                <div class="column-content style-text">
                    <h3>TAGS</h3>
                    <div class="tags-container">
                        <span class="tag-card" v-for="(tag, index) in tags" :key="index">
                            <a :href="tag.url">{{tag.text}}</a>
                        </span>
                    </div></div>   
        </div>
    </div>
    <div class="bottom-footer-container">
        <div class="btm-content">
            <div class="btm-text">
                <span>
                    <i class="fa-regular fa-copyright"></i>
                    Copyright 2012 - 2020
                </span> |
                <span>
                    Avada Theme by Theme Fusion
                </span> |
                <span>
                    All Rights Reserved
                </span> |
                <span>
                    Powered by Wordpress
                </span>
            </div>
            <div class="btm-images">
                <img src="../assets/img/payment_cards_footer.png">
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'MyFooter',
    data() {
    return {
      topRated: [
                {
                    url: 'leather_gloves-120x156.jpg',
                    product: "Leather Gloves",
                    ratings: "5",
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
                    ratings: "5",
                    price: "$47"
                },
            ],
            tags: [
                {
                    text: "Black",
                    url: "#",
                },
                {
                    text: "boots",
                    url: "#",
                },
                {
                    text: "Brown",
                    url: "#",
                },
                {
                    text: "Casual",
                    url: "#",
                },
                {
                    text: "D&G",
                    url: "#",
                },
                {
                    text: "Fabric",
                    url: "#",
                },
                {
                    text: "flowers",
                    url: "#",
                },
                {
                    text: "grey",
                    url: "#",
                },
                {
                    text: "hat",
                    url: "#",
                },
                {
                    text: "Hipster",
                    url: "#",
                },
                {
                    text: "lines",
                    url: "#",
                },
                {
                    text: "multi-purpose",
                    url: "#",
                },
                {
                    text: "New York",
                    url: "#",
                },
                {
                    text: "Outdoors",
                    url: "#",
                },
                {
                    text: "red",
                    url: "#",
                },
                {
                    text: "responsive",
                    url: "#",
                },
                {
                    text: "summer",
                    url: "#",
                },
                {
                    text: "sweater",
                    url: "#",
                },
                {
                    text: "Travel",
                    url: "#",
                },
                {
                    text: "warm",
                    url: "#",
                },
                {
                    text: "White",
                    url: "#",
                },
                {
                    text: "winter",
                    url: "#",
                },
            ],
        }
    },
    props: {
        infos: Object
    },
}
</script>

<style scoped>
@import "../assets/style/myfooter.scss";
</style>