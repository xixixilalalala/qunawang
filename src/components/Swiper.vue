<template>
    <div class="wrapper">
        <swiper :options="swiperOption"  >
    <!-- slides -->
    <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl" alt="">
    </swiper-slide>
    <!-- Optional controls -->
    <div class="swiper-pagination"  slot="pagination"></div>
  </swiper>
  </div>
</template>
    
<script setup lang='ts'>
    export default{
        name:'HomeSwiper',
        data (){
            return{
                swiperOption:{
                    pagination: 
                        '.swiper-pagination',
                    loop:true
                },
                swiperList:[{
                    id:'0001',
                    imgUrl:"https://tr-osdcp.qunarzz.com/tr-osd-vs-dapp-ugc/img/edbaff9644f3df8109252700f911f437.jpg"
                },{
                    id:'0002',
                    imgUrl:"https://tr-osdcp.qunarzz.com/tr-osd-vs-dapp-ugc/img/eb573103e9890780fce51b524a3d61e4.jpg"
                }
                ]
            }
        }
    }
</script>
    
<style lang="stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active{
    background: #fff
}
.wrapper{
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 31.25%
    background: #eee
     .swiper-img{
        width: 100%
    }
}
   
</style>