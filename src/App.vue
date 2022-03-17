<template>
    <div>
      <home-header />
      <home-swiper />
    </div>
</template>
  
<script setup lang='ts'>
import HomeHeader from './components/Header.vue'
import HomeSwiper from './components/Swiper.vue'
  export default{
    name:'App',
    components:{
      HomeHeader,
      HomeSwiper
    }
  }
</script>
  
<style>
  
</style>
