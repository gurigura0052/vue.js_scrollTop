<template>
  <div id="app">
    <header id="top">
      #top
    </header>
    <scroll-top/>
  </div>
</template>

<script>
import Vue from 'vue'
import scrollTop from '@/components/scrollTop'

Vue.component('scroll-top', scrollTop)

export default {
  name: 'app'
}
</script>

<style>
html{
  height: 100%;
}
body{
  height: 200%;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
