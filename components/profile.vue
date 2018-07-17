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
        .profile-label 趣味：
        .profile-hobby ギター
      .profile-list
        .profile-label 資格：
        .profile-qualiflcation 基本情報
        // アイコン使用
      .profile-sns
        .profile-twitter
          a.twitter-link
            i
        .profile-github
          a.github-link
            i
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
    margin: 0 auto 50px auto;
    border-radius: 50%;
    @include desktop() {
      width: 250px;
      height: 250px;
    }
  }
  &-list {
    margin-bottom: 20px;
    border-bottom: 5px solid $green;
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
}
</style>