<template>
  <div class="swiper">
    <swiper class="swiper-swiper" ref="mySwiper" :options="swiperOptions">
      <swiper-slide v-for="(item, index) in swiperList" :key="index">
        <img class="swiper-img" :src="item.imgSrc" />
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>
<script>
export default {
  name: "HomeSwiper",
  data() {
    return {
      swiperOptions: {
        pagination: {
          el: ".swiper-pagination",
        },
        autoplay: true, // Some Swiper option/callback...
        loop: true,
      },
      swiperList: [
        {
          id: "001",
          imgSrc:
            "//img1.qunarzz.com/sight/p0/201405/27/544cae2aeb173cb6533ce6926b68f153.jpg_256x160_e80a446b.jpg",
        },
        {
          id: "002",
          imgSrc:
            "//img1.qunarzz.com/sight/p65/201211/07/2dcda4e400ace9f993835fbb.jpg_256x160_b1a93ad3.jpg",
        },
        {
          id: "003",
          imgSrc:
            "//img1.qunarzz.com/sight/p0/1709/e9/e9b7ae23f567806ea3.img.jpg_256x160_659f7c33.jpg",
        },
        {
          id: "004",
          imgSrc:
            "//img1.qunarzz.com/sight/p0/1701/88/885ec9c1584a572aa3.img.png_256x160_cdccb910.png",
        },
      ],
    };
  },
  computed: {
    swiper() {
      return this.$refs.mySwiper.$swiper;
    },
  },
  mounted() {
    console.log("Current Swiper instance object", this.swiper);
    this.swiper.slideTo(0, 1000, false);
  },
};
</script>
<style type='text/css' scoped>
.swiper {
  overflow: hidden;
  height: 0;
  padding-bottom: 3rem;
}
.swiper-swiper {
  width: 100%;
}
.swiper-img {
  width: 100%;
}
</style>