<template lang="pug">
  main.p-product
    h3.product-title 作品
    .product-list
      a.product-link(href=""): i  BookShelf
      .product-img
    .product-list
      a.product-link(href=""): i ChatMammoss
      .product-img
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
    color: #000;
    font-weight: bold;
  }
}
</style>