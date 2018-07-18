<template lang="pug">
  header.l-header
    .st-container
      h1.header-title MySite
      .menu
        label(for="menu")
          i.fas.fa-bars
        input.on-off(type="checkbox" id="menu")
        ul.menu-list
          li
            a(href="/") トップ
          li
            a(href="/profile") プロフィール
          li
            a(href="/product") 作品
</template>

<script>
</script>

<style lang="scss" spend>
@import "~assets/scss/library/mixin.scss";

.l-header {

}

.st-container {
  position: relative;
}

.header-title {
  display: inline-block;
  margin: 0;
  line-height: 80px;
  @include desktop() {
    line-height: 100px;
  }
}

.menu {
  display: inline-block;
  position: absolute;
  top: 27px;
  right: 10px;
  @include desktop() {
    top: 50%;
    transform: translateY(-50%);
  }
  label {
    display: block;
    margin: 0;
    text-align: right;
    @include desktop() {
      display: none;
    }
    i {
      font-size: 26px;
    }
  }
  .on-off{
    display: none;
  }
  &-list {
    position: relative;
    right: -10px;
    transition: 0.5s;
    margin: 0;
    padding: 0;
    list-style: none;
    height: 0;
    overflow: hidden;
    z-index: 999;
    @include desktop() {
      position: static;
      height: auto;
    }
    li {
      padding: 5px;
      z-index: 1000;
      @include desktop() {
        display: inline-block;
      }
      a {
        color: #333;
        text-decoration: none;
        display: inline-block;
        width: 100%;
        cursor: pointer;
      }
    }
  }
  .on-off:checked + ul{
    height: 102px;
  }
}

.menu-list {
  a {
    cursor: pointer;
  }
}
</style>