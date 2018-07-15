<template lang="pug">
  main.p-main
    .a-circle
</template>

<script>

</script>

<style lang="scss" scoped>
@import "~assets/scss/library/mixin.scss";
@import "~assets/scss/library/variable.scss";

.p-main {
  position: relative;
}

.a-circle {
  position: absolute;
  width: 100px;
  height: 100px;
  border-radius: 50%;
  background: #0aa;
  top: 50%;
  left: 50%;
  transform: translateX(-50%);
  transform-origin: 0 0;
  animation: circle 10s infinite;
}
  
@keyframes circle {
  0% {
    width: 100px;
    height: 100px;
  }
  50% {
    width: 0;
    height: 0;
  }
  100% {
    width: 100px;
    height: 100px;
  }
}

</style>