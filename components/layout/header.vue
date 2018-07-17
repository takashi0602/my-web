<template lang="pug">
  header.l-header
    h1.header-title MySite
    .menu
      label(for="menu")
        i.material-icons dehaze
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
  position: relative;
}

.header-title {
  display: inline-block;
  margin: 0;
  line-height: 100px;
}

.menu {
  display: inline-block;
  position: absolute;
  top: 30px;
  right: 10px;
  label {
    display: block;
    margin: 0;
    color: #000;
    text-align: right;
    @include desktop() {
      display: none;
    }
    i {
      font-size: 40px;
    }
  }
  .on-off{
    display: none;
  }
  &-list {
    transition: 0.5s;
    margin: 0;
    padding: 0;
    list-style: none;
    height: 0;
    overflow: hidden;
    z-index: 1000;
    @include desktop() {
      height: auto;
    }
    li {
      padding: 5px;
      @include desktop() {
        display: inline-block;
      }
      a {
        color: black;
        text-decoration: none;
      }
    }
  }
  .on-off:checked + ul{
    height: 200px;
  }
}

.menu-list {
  a {
    cursor: pointer;
  }
}
</style>