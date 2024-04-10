<script>
import HomeHeader from './components/HomeHeader.vue'
import HomeMain from './components/HomeMain.vue'
import HomeFooter from './components/HomeFooter.vue'

export default {
  components: {
    HomeHeader,
    HomeMain,
    HomeFooter
  }
}
</script>

<template>
  <HomeHeader />
  <HomeMain />
  <HomeFooter />
</template>

<style lang="scss">
@use './style/general';
</style>
