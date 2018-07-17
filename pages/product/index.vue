<template lang="pug">
  section
    .st-container
      l-header
      p-product
</template>

<script>
  import lHeader from '~/components/layout/header.vue'
  import pProduct from '~/components/product.vue'

  export default {
    components: {
      lHeader,
      pProduct
    }
  }
</script>

<style lang="scss">
@import "~assets/scss/foundation/base.scss";
@import "~assets/scss/object/common.scss";
</style>