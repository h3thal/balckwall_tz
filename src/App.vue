<template>
  <div id="circle"></div>
  <Navbar/>
  <Home/>
</template>

<script>
import Navbar from './components/Nav/Navbar.vue'
import Home from './components/Home/Home.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Home
  }
}
</script>

<style lang="scss">
  #circle {
    position: absolute;
    width: 766px;
    height: 766px;
    left: -149px;
    top: -147px;
    background: #FF523D;
    opacity: 0.05;
    filter: blur(150px);
    z-index: -5;
  }
</style>
