<template>
    <div class="container-ft-products">
        <div class="ft-products-sec">
            <div class="title-ft-products">
                <h2>From Our Blog</h2>
            </div>
            <span>The latest Classic Shop news</span>
        </div>
        <div class="blog-content">
            <div class="blog-column" v-for="(content, index) in contents" :key="index">
                <img :src="require(`../assets/img/` + content.url)">
                <div class="title">{{content.title}}</div>
                <span class="date">{{content.date}}</span> | <span class="comments">{{content.comments}}</span>
                <p class="snippet">{{content.snippet}}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FromOurBlog',
    data() {
    return {
      contents: [
          {
              url: 'post_img_12-320x202.jpg',
              title: "Aenean lobortis sapienenim viverra",
              date: "September 9th, 2015",
              comments: "0 Comments",
              snippet: "Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla."
          },
          {
              url: 'post_img_11-320x202.jpg',
              title: "Aenean lobortis sapienenim viverra",
              date: "September 9th, 2015",
              comments: "0 Comments",
              snippet: "Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla."
          },
          {
              url: 'post_img_10-320x202.jpg',
              title: "Aenean lobortis sapienenim viverra",
              date: "September 9th, 2015",
              comments: "0 Comments",
              snippet: "Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla."
          },
      ],
    }
  }
}
</script>

<style scoped>
@import "../assets/style/fromourblog.scss";
</style>