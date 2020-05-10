<template>
  <div class="wrapper">
    <swiper ref="mySwiper" :options="swiperOptions">
      <swiper-slide v-for="item in swiperList" :key="item.id">
        <img
          class="swiper-image"
          :src="item.img_url"/>
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
      <div>test</div>
    </swiper>
  </div>
</template>

<script>
    export default {
          name: "HomeSwiper",
          data(){
            return {
              swiperOptions:{
                pagination:'.swiper-pagination',
                loop:true
              },
              swiperList:[{
                id:'001',
                img_url:"http://www.bizhidaquan.com/d/file/1/1159829.jpg"
              },{
                id:'001',
                img_url:"http://www.bizhidaquan.com/d/file/1/1159829.jpg"
              }
              ]
            }
          }
    }
</script>

<style scoped lang="stylus">
  .wrapper >>> .swiper-pagination-bullet-active
    background :white !important

  .wrapper
    overflow :hidden
    width :100%
    height:0
    padding-bottom:66%
    background white
    .swiper-image
      width :100%

</style>
