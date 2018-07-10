<template lang="pug">
  .st-container
    header.l-header
      h1 Idol Is God
      .menu
        label(for="menu") ボタン1
        input.on-off(type="checkbox" id="menu")
        ul
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

<style lang="scss" scoped>
@import "~assets/scss/foundation/base.scss";
@import "~assets/scss/object/common.scss";

.menu {
  label {
    background: green;
    color: #fff;
    padding: 10px;
    display: block;
    margin: 0;
    border: 1px solid #fff;
  }
  .on-off{
    display: none;
  }
  ul {
    transition: 0.5s;
    margin: 0;
    padding: 0;
    list-style: none;
    height: 0;
    overflow: hidden;
    li {
      padding: 5px;
    }
  }
  .on-off:checked + ul{
    height: 200px;
  }
}
</style>
