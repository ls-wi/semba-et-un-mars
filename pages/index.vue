<template>
  <div>
    <Header/>
    <MainHero class="main-hero" v-bind:hero="hero"/>

  </div>
</template>

<script>
import Header from '../components/Header.vue';
import MainHero from '@/components/MainHero';
export default {
  name: 'IndexPage',
  components:{
    Header,
    MainHero
  },
  data() {
    return {
      hero: {
          imageHD : "images/main_seum.jpg",
          imageM : "images/main_seum.jpg",
          imageLD : "images/main_seum.jpg",
          titre : "Podcasts",
          filtre: "green"
      }
    }
  }
}
</script>
