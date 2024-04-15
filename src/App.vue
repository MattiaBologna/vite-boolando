<script>
import HomeHeader from './components/HomeHeader.vue'
import HomeMain from './components/HomeMain.vue'
import HomeFooter from './components/HomeFooter.vue'
import axios from 'axios';
import { store } from './store.js';

export default {
  created() {
    this.fetchData()
  },
  components: {
    HomeHeader,
    HomeMain,
    HomeFooter
  },
  methods: {
    fetchData() {
      axios.get('http://localhost:3000/products').then((res) => {
        console.log('ress: ', res.data)
        console.log('pre-store> ', store)
        store.products = res.data
      })
    }
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
