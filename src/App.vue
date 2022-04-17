<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Loader from './components/Loader.vue'

</script>

<template>
  <Loader />
  <Header/>
  <RouterView />
  <Footer />
</template>

<style lang="scss">
@import '@/assets/style.scss';


</style>
<script>
export default {
  components: {
    Header,
    Footer,
    Loader
  }
}

</script>