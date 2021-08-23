<template>
  <div id="information">
    <div class="wrapper">
      <div class="information-row">
        <div class="information-row__left">
          Collaborate 2M+ startup and international companies ueses since 2018
        </div>
        <div class="information-row__right">
          <div class="block">
            <div class="title">15k</div>
            <div class="icons">
              <img v-for="icon in 5" :key="icon" src="@/assets/heart.svg" alt="">
            </div>
            <div class="subtitle">Active Downloads</div>
          </div>
          <div class="block">
            <div class="title">4.9</div>
            <div class="icons">
              <img v-for="icon in 5" :key="icon" src="@/assets/star.svg" alt="">
            </div>
            <div class="subtitle">2,938 Rating</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import '@/assets/scss/__extends.scss';
@import '@/assets/scss/__fonts.scss';
@import '@/assets/scss/__mixin.scss';
#information {
  .wrapper {
    .information-row {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      @include lg {
        flex-direction: column;
      }
      &__left {
        font-family: Inter;
        font-style: normal;
        font-weight: 600;
        font-size: 36px;
        line-height: 50px;
        color: $navyBlue;
        width: 600px;
      }
      &__right {
        width: 300px;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        .block {
          .title {
            font-family: Inter;
            font-style: normal;
            font-weight: bold;
            font-size: 60px;
            line-height: 70px;
            color: $navyBlue;
          }
          .icons {
            display: flex;
            justify-content: space-evenly;
            width: 100px;
            margin: 10px 0px 12px;
          }
          .subtitle {
            font-family: Inter;
            font-style: normal;
            font-weight: normal;
            font-size: 16px;
            line-height: 28px;
            color: $navyBlue;
          }
        }
      }
    }
  }
}
</style>
