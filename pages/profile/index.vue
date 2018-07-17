<template lang="pug">
  section
    l-header
    .st-container
      p-profile
</template>

<script>
  import lHeader from '~/components/layout/header.vue'
  import pProfile from '~/components/profile.vue'

  export default {
    components: {
      lHeader,
      pProfile
    }
  }
</script>

<style lang="scss">
@import "~assets/scss/foundation/base.scss";
@import "~assets/scss/object/common.scss";
</style>