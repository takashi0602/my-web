<template lang="pug">
  .st-container
    header.l-header
      h1.header-title Idol Is God
      .menu
        label(for="menu")
          i.material-icons dehaze
        input.on-off(type="checkbox" id="menu")
        ul.menu-list
          li
            a(href="") リンク1
          li
            a(href="") リンク2
          li
            a(href="") リンク3
          li
            a(href="") リンク4
    nuxt
</template>

<style lang="scss">
@import "~assets/scss/foundation/base.scss";
@import "~assets/scss/object/common.scss";

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
  top: 28px;
  right: 0;
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

.menu_pc {
  display: none;
  @include desktop() {
    display: inline-block;
    position: absolute;
    right: 0;
    top: 50%;
    transform: translateY(-50%);
  }
  .c-link {
    display: inline-block;
    padding-left: 10px;
    a {
      text-decoration: none;
      color: black;
    }
  }
}
</style>
