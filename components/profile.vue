<template lang="pug">
  main.p-profile
    h3.profile-title プロフィール
    .profile-img
    .profile-area
      .profile-list
        .profile-label 名前：
        .profile-name たかし
      .profile-list
        .profile-label 生年月日：
        .profile-birthday 1998/06/02
      .profile-list
        .profile-label 資格：
        .profile-qualiflcation 基本情報技術者試験
      .profile-list
        .profile-label 推し：
        .profile-hobby 小池美波 あの(ゆるめるモ!)
      .profile-sns
        .profile-twitter
          a.twitter-link(href="https://twitter.com/aJDHpAglNUJepZ9" target="_blank")
            i.fab.fa-twitter
        .profile-github
          a.github-link(href="https://github.com/takashi0602" target="_blank")
            i.fab.fa-github
  </span>
</template>

<script>
</script>

<style lang="scss" scoped>
@import "~assets/scss/library/mixin.scss";

.profile {
  font-size: 18px;
  &-area {
    width: 100%;
    max-width: 480px;
    margin: 0 auto;
  }
  &-title {
    font-size: 24px;
  }
  &-img {
    width: 150px;
    height: 150px;
    background-image: url("~static/images/takashi.png");
    background-repeat: no-repeat;
    background-size: contain;
    margin: 0 auto 20px auto;
    border: 7px solid $green;
    border-radius: 50%;
    @include desktop() {
      width: 250px;
      height: 250px;
      margin: 0 auto 50px auto;
      border: 10px solid $green;
    }
  }
  &-list {
    margin-bottom: 15px;
    border-bottom: 3px solid $green;
    @include desktop() {
      margin-bottom: 20px;
      border-bottom: 5px solid $green;
    }
  }
  &-label {
    display: inline-block;
  }
  &-name {
    display: inline-block;
  }
  &-birthday {
    display: inline-block;
  }
  &-hobby {
    display: inline-block;
  }
  &-qualiflcation {
    display: inline-block;
  }
  &-sns {
    text-align: center;
  }
  &-twitter {
    display: inline-block;
    margin-right: 10px;
  }
  &-github {
    display: inline-block;
    margin-left: 10px;
  }
}

.twitter-link {
  text-decoration: none;
  cursor: pointer;
  i {
    color: #00aced;
    font-size: 30px;
    @include desktop() {
      font-size: 40px;
    }
  }
}

.github-link {
  text-decoration: none;
  cursor: pointer;
  i {
    color: #333;
    font-size: 30px;
    @include desktop() {
      font-size: 40px;
    }
  }
}
</style>