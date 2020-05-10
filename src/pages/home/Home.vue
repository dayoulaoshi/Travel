<template>
  <div>
    <HomeHeader></HomeHeader>
    <HomeSwiper></HomeSwiper>
  </div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwiper from "./components/Swiper";
export default {
  name: 'Home',
  components:{
    HomeSwiper,
    HomeHeader
  }

}
</script>

<style scoped>

</style>
