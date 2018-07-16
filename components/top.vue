<template lang="pug">
  main.p-top
    .a-area
      .a-circle
      .st-container
        .a-word
          .a-word1
            span M
          .a-word2
            span y
          .a-word3
            span S
          .a-word4
            span i
          .a-word5
            span t
          .a-word6
            span e
    .top-container
      .top-list
        .top-img
        .top-links
          a.top-link1(href="/profile") プロフィール
          a.top-link2(href="/product") 作品
</template>

<script>
</script>

<style lang="scss" scoped>
@import "~assets/scss/library/mixin.scss";

.a-area {
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  background: $yellow;
  opacity: 1;
  animation: display1 3s 12s 1 forwards;
}

@keyframes display1 {
  0% {
    opacity: 1;
    height: 100vh;
    visibility: visible;
  }
  99% {
    opacity: 0;
    height: 100vh;
    visibility: hidden;
  }
  100% {
    height: 0;
    visibility: hidden;
  }
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
.st-container {
  position: fixed;
  top: 0;
  height: 100vh;
}
.a-word {
  position: absolute;
  width: 100%;
  height: 415px;
  top: 50%;
  transform: translateY(-50%);
  font-size: 36px;
  color: #fff;
  font-weight: bold;
  @include desktop() {
    display: inline-block;
    font-size: 60px;
    height: 100px;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  &1 {
    position: absolute;
    top: 0;
    right: 20%;
    width: 75px;
    height: 75px;
    border-radius: 50%;
    background: $red;
    transform: scale(0, 0);
    animation: word1 2s 5s 1 forwards;
    @include desktop() {
      top: 0;
      left: 34px;
      width: 100px;
      height: 100px;
    }
    span {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
  }
  &2 {
    position: absolute;
    top: 85px;
    right: 20%;
    width: 75px;
    height: 75px;
    border-radius: 50%;
    background: $blue;
    transform: scale(0, 0);
    animation: word1 2s 6s 1 forwards;
    @include desktop() {
      top: 0;
      left: 154px;
      width: 100px;
      height: 100px;
    }
    span {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
  }
  &3 {
    position: absolute;
    top: 85px;
    left: 20%;
    width: 75px;
    height: 75px;
    border-radius: 50%;
    background: $lightblue;
    transform: scale(0, 0);
    animation: word1 2s 7s 1 forwards;
    @include desktop() {
      top: 0;
      left: 274px;
      width: 100px;
      height: 100px;
    }
    span {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
  }
  &4 {
    position: absolute;
    top: 170px;
    left: 20%;
    width: 75px;
    height: 75px;
    border-radius: 50%;
    background: $orange;
    transform: scale(0, 0);
    animation: word1 2s 8s 1 forwards;
    @include desktop() {
      top: 0;
      left: 394px;
      width: 100px;
      height: 100px;
    }
    span {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
  }
  &5 {
    position: absolute;
    top: 255px;
    left: 20%;
    width: 75px;
    height: 75px;
    border-radius: 50%;
    background: $yellowgreen;
    transform: scale(0, 0);
    animation: word1 2s 9s 1 forwards;
    @include desktop() {
      top: 0;
      left: 514px;
      width: 100px;
      height: 100px;
    }
    span {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
  }
  &6 {
    position: absolute;
    top: 340px;
    left: 20%;
    width: 75px;
    height: 75px;
    border-radius: 50%;
    background: $purple;
    transform: scale(0, 0);
    animation: word1 2s 10s 1 forwards;
    @include desktop() {
      top: 0;
      left: 634px;
      width: 100px;
      height: 100px;
    }
    span {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
  }
}

@keyframes word1 {
  0% {
    transform: scale(0, 0);
  }
  75% {
    transform: scale(1.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}

.top {
  &-container {
    position: relative;
    width: 0;
    height: 0;
    overflow: hidden;
    opacity: 0;
    background: $yellow;
    animation: display2 3s 16s 1 forwards;
  }
  &-list {
    position: absolute;
    width: 500px;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  &-img {
    width: 150px;
    height: 150px;
    background-image: url("~static/images/takashi.png");
    background-repeat: no-repeat;
    background-size: contain;
    margin: 0 auto 20px auto;
    border-radius: 50%;
    @include desktop() {
      width: 300px;
      height: 300px;
    }
  }
  &-link1 {
    display: block;
    text-align: center;
    width: 150px;
    background: $red;
    cursor: pointer;
    margin: 0 auto 20px auto;
    padding: 5px 0;
    border-radius: 20px;
    color: #fff;
    text-decoration: none;
    @include desktop() {
      display: inline-block;
      width: 200px;
      margin: 0 20px;
      font-size: 24px;
      border-radius: 30px;
      transform: scale(1, 1);
    }
  }
  &-link1:hover {
    transition: 0.5s;
    transform: scale(1.2, 1.2);
  }
  &-link2 {
    display: block;
    text-align: center;
    width: 150px;
    background: $blue;
    cursor: pointer;
    margin: 0 auto;
    padding: 5px 0;
    border-radius: 20px;
    color: #fff;
    text-decoration: none;
    @include desktop() {
      display: inline-block;
      width: 200px;
      margin: 0 20px;
      font-size: 24px;
      border-radius: 30px;
    }
  }
  &-link2:hover {
    transition: 0.5s;
    transform: scale(1.2, 1.2);
  }
}

@keyframes display2 {
  0% {
    width: 0;
    height: 0;
    opacity: 0;
    visibility: hidden;
  }
  1% {
    width: 100vw;
    height: 100vh;
    opacity: 0;
    visibility: hidden;
  }
  100% {
    width: 100vw;
    height: 100vh;
    opacity: 1;
    visibility: visible;
  }
}
</style>