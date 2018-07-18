<template lang="pug">
  main.p-product
    h3.product-title 作品
    .product-list
      a.product-link(href="https://b00kshe1f.herokuapp.com/" target="_blank") Bookshelf
      p.product-description - 本を管理するためのアプリ
      a.product-img1(href="https://b00kshe1f.herokuapp.com/" target="_blank")
    .product-list
      a.product-link(href="https://chat-mammoth.herokuapp.com/" target="_blank") chat mammoth
      p.product-description - チャットを楽しむアプリ
      a.product-img2(href="https://chat-mammoth.herokuapp.com/" target="_blank")
</template>

<script>
</script>

<style lang="scss" scoped>
@import "~assets/scss/library/mixin.scss";

.product {
  font-size: 18px;
  &-title {
    font-size: 24px;
  }
  &-link {
    text-decoration: none;
    cursor: pointer;
    color: #333;
    font-weight: bold;
    font-size: 20px;
  }
  &-img1 {
    display: inline-block;
    cursor: pointer;
    width: 100%;
    height: 240px;
    background-image: url("~static/images/bookshelf.png");
    background-repeat: no-repeat;
    background-size: contain;
    border-radius: 10px;
    @include desktop() {
      height: 480px;
    }
  }
  &-img2 {
    display: inline-block;
    cursor: pointer;
    width: 100%;
    height: 240px;
    background-image: url("~static/images/chat-mammoth.png");
    background-repeat: no-repeat;
    background-size: contain;
    border-radius: 10px;
    @include desktop() {
      height: 480px;
    }
  }
}
</style>