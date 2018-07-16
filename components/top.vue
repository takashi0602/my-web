<template lang="pug">
  main.p-main
    .a-circle
    .word
      .word1 M
      .word2 y
      .word3 S
      .word4 i
      .word5 t
      .word6 e
</template>

<script>

</script>

<style lang="scss" scoped>
@import "~assets/scss/library/mixin.scss";

.p-main {
  width: 100vw;
  height: 100vh;
  min-height: 100vh;
  overflow: hidden;
  background: $yellow;
}

.a-circle {
  position: relative;
  width: 100px;
  height: 100px;
  border-radius: 50%;
  background: $green;
  border: none;
  top: 50%;
  left: 50%;
  transform-origin: center;
  transform: translate(-50%, -50%) scale(50, 50);
  animation: circle 4s 1 forwards;
}

@keyframes circle {
  0% {
    transform: translate(-50%, -50%) scale(50, 50);
  }
  100% {
    transform: translate(-50%, -50%) scale(0, 0);
  }
}

.word {
  position: relative;
  @include desktop() {
    display: inline-block;
  }
  &1 {
    position: absolute;
    @include desktop() {

    }
  }
  &2 {
    position: absolute;
    @include desktop() {

    }
  }
  &3 {
    position: absolute;
    @include desktop() {

    }
  }
  &4 {
    position: absolute;
    @include desktop() {

    }
  }
  &5 {
    position: absolute;
    @include desktop() {

    }
  }
  &6 {
    position: absolute;
    @include desktop() {

    }
  }

}

</style>