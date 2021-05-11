<template>
  <div>
    
    <!--中间的滚动部分-->
    <div class="wrapper list" ref="wrapper">
      <div class="content">
        <div class="list-title">当前城市</div>
        <div class="list-content">
          <div class="list-current">北京</div>
          <div class="list-current">北京</div>
          <div class="list-current">北京</div>
          <div class="list-current">北京</div>
          <div class="list-current">北京</div>
        </div>
        <div class="list-title">热门城市</div>
        <div class="list-content">
          <div class="list-current">北京</div>
          <div class="list-current">北京</div>
          <div class="list-current">北京</div>
          <div class="list-current">北京</div>
          <div class="list-current">北京</div>
          <div class="list-current">北京</div>
        </div>
        <div class="list-title">A</div>
        <div class="list-countent">
          <div class="list-item">阿拉善</div>
          <div class="list-item">阿拉善</div>
          <div class="list-item">阿拉善</div>
          <div class="list-item">阿拉善</div>
          <div class="list-item">阿拉善</div>
          <div class="list-item">阿拉善</div>
          <div class="list-item">阿拉善</div>
          <div class="list-item">阿拉善</div>
        </div>
        <div class="list-title">A</div>
        <div class="list-countent">
          <div class="list-item">阿拉善</div>
          <div class="list-item">阿拉善</div>
          <div class="list-item">阿拉善</div>
          <div class="list-item">阿拉善</div>
          <div class="list-item">阿拉善</div>
          <div class="list-item">阿拉善</div>
          <div class="list-item">阿拉善</div>
          <div class="list-item">阿拉善</div>
        </div>
      </div>
    </div>

    <!--字母列表-->
    <div class="list-letter">
      <div clas="list-letter-item">A</div>
      <div clas="list-letter-item">A</div>
      <div clas="list-letter-item">A</div>
      <div clas="list-letter-item">A</div>
      <div clas="list-letter-item">A</div>
      <div clas="list-letter-item">A</div>
      <div clas="list-letter-item">A</div>
      <div clas="list-letter-item">A</div>
      <div clas="list-letter-item">A</div>
      <div clas="list-letter-item">A</div>
      <div clas="list-letter-item">A</div>
    </div>
  </div>
</template>
<script>
import BScroll from "@better-scroll/core";
export default {
  name: "CityList",
  data() {
    return {};
  },
  mounted() {
    this.$nextTick(() => {
      this.scroll = new BScroll(this.$refs.wrapper, {});
      this.scroll.refresh();
    });
  },
};
</script>
<style scoped>
.list {
  position: absolute;
  top: 1.6rem;
  left: 0;
  right: 0;
  bottom: 0;
  overflow: hidden;
}
.list-title {
  background-color: rgb(245, 240, 240);
  color: #333;
  border-bottom: 1px solid rgb(218, 215, 215);
  padding: 0.1rem 0.2rem;
}
.list-current {
  border: 1px solid rgb(195, 192, 192);
  color: #333;
  width: 28%;
  border-radius: 0.1rem;
  padding: 0.1rem 0;
  margin: 0.2rem 0.1rem;
  text-align: center;
  display: inline-block;
}
.list-content {
  margin-right: 0.3rem;
}
.list-item {
  color: #333;
  border-bottom: 1px solid rgb(230, 226, 226);
  padding: 0.2rem 0.2rem;
}
.list-letter {
  position: fixed;
  top: 3rem;
  right: 0.1rem;
  color: #00bcd4;
  z-index: 2;
}
</style>