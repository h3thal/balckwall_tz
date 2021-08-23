<template>
  <div id="slider">
    <div class="wrapper">
      <img src="@/assets/1.png" alt="" class="item">
      <img src="@/assets/2.png" alt="" class="item">
      <img src="@/assets/3.png" alt="" class="item">
      <img src="@/assets/4.png" alt="" class="item">
      <img src="@/assets/5.png" alt="" class="item">
      <img src="@/assets/6.png" alt="" class="item">
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '@/assets/scss/__extends.scss';
@import '@/assets/scss/__mixin.scss';
#slider {
  .wrapper {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    overflow-x: hidden;
    .item {
    }
  }
}
</style>
