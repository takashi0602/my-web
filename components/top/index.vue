<template lang="pug">
  main.p-main
    .st-container
      h1 Idol Is God
      p.p-main_balloon 僕の推しを紹介するサイト
      .p-main_img
</template>

<script>

</script>

<style lang="scss" scoped>
@import "~assets/scss/library/mixin.scss";
@import "~assets/scss/library/variable.scss";

.p-main {
  color: #0099aa;
  &_balloon {
    color: #fff;
    font-weight: bold;
    display: inline-block;
    position: relative;
    background: #0099ee;
    border-radius: 30px;
    padding: 10px 15px;
  }
  &_balloon:before {
    content: "";
    display: block;
    margin-left: -10px;
    border: 10px solid transparent;
    border-left: 30px solid #0099ee;
    position: absolute;
    top: 85%;
    left: 15%;
    transform: rotate(45deg);
    z-index: -1;
  }
  &_img {
    background-image: url("/images/penguin_1.svg");
    background-repeat: no-repeat;
    background-size: contain;
    width: 200px;
    height: 200px;
    position: relative;
    top: -10px;
    left: 5%;
  }
}

</style>