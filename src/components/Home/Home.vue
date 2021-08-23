<template>
  <div id="home">
    <div class="wrapper">
      <div class="home__block">
        <div class="home__block-title">
          The best video online meeting software.
        </div>
        <div class="home__block-subtitle">
          Many desktop publishing packages and web page editors now use Lorem Ipsum as their default
        </div>
        <div class="home__block-button">
          Start for free
        </div>
      </div>
      <img class="pc" src="@/assets/home.png" alt="">
      <img class="mobile" src="@/assets/mobile.png" alt="">
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
#home {
  height: 520px;
  .wrapper {
    position: relative;
    height: 100%;
    .home__block {
      height: 100%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      width: 50%;
      @include lg {
        text-align: center;
        align-items: center;
        margin: auto;
      }
      &-title {
        color: $navyBlue;
        font-family: Inter;
        font-style: normal;
        font-weight: 600;
        font-size: 48px;
        line-height: 60px;
        width: 498px;
      }
      &-subtitle {
        color: $navyBlue;
        font-family: Inter;
        font-style: normal;
        font-weight: normal;
        font-size: 17px;
        line-height: 28px;
        width: 484px;
      }
      &-button {
        color: $navyBlue;
        font-family: Inter;
        font-style: normal;
        font-weight: 500;
        font-size: 17px;
        line-height: 21px;
        background-color: $neonBlue;
        width: 180px;
        height: 66px;
        border-radius: 6px;
        display: flex;
        align-items: center;
        justify-content: center;
        cursor: pointer;
      }
    }
    img.pc {
      position: absolute;
      top: 0px;
      right: 0px;
      display: flex;
      @include lg {
        display: none;
      }
    }
    img.mobile {
      display: none;
      width: 300px;
      margin: auto;
      @include lg {
        display: flex;
      }
    }
  }
}
</style>
