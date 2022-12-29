<template>
    <div v-bind:class="[mainHero, isRaptzPage ? mainHeroAfter : null]">
      <picture v-if="hero.imageM">
        <source class="main-hero__img" media="(max-width: 789px)" v-bind:srcset="require(`@/assets/${hero.imageLD}`)">
        <source class="main-hero__img" media="(min-width: 1400px)" v-bind:srcset="require(`@/assets/${hero.imageHD}`)">
        <img class="main-hero__img" v-bind:src="require(`@/assets/${hero.imageM}`)" alt="Raptz hero image">
      </picture>
      <div v-else class="main-hero__alt-background"></div>
      <div v-if="hero.filtre=='red'" class='filtre-red'></div>
      <div v-if="hero.filtre=='blue'" class='filtre-blue'></div>
      <div v-if="hero.filtre=='green'" class='filtre-green'></div>
      <div class="main-hero__titre-container" v-if="hero.titre!=''">
      </div>
  </div>

</template>

<style>

  .main-hero {
    overflow:hidden;
    position:relative;
    height:30em;
    z-index:-1;
    border-bottom: 3px solid #2d7e3e;
  }
  

  .main-hero__img {
    width: 100%;
    height:auto;
    height:30em;
    object-fit: cover;
    z-index:-1;
  }

  .main-hero__titre-container {
    position: absolute;
    width:100%;
    text-align:center;
    top: 243px;

  }

  .main-hero__titre {
    max-width: 704px;
    margin:auto auto;
    height: 61px;
    text-align:center;

    font-family: Chau Philomene One;
    font-style: normal;
    font-weight: normal;
    font-size: 45px;
    line-height: 140%;

    /* or 63px */
    letter-spacing: 0.01em;
    text-transform: uppercase;

    color: #FCFAFA;

    text-shadow: 0px 1px 2px rgba(0, 0, 0, 0.25);
  }

  .main-hero__alt-background {
    background-color: #233045 ;
    width:100%;
    height:100%;
  }

  .filtre-red {
    position:absolute;
    top:0;
    left:0;
    width:100%;
    height:100%;
    background: linear-gradient(215.81deg, rgba(20, 52, 62, 0.38) 19.04%, rgba(37, 88, 99, 0.5) 34.07%, rgba(165, 24, 41, 0.48) 67.05%);
  }

  .filtre-blue{
    position:absolute;
    top:0;
    left:0;
    width:100%;
    height:100%;
    background: linear-gradient(180deg, rgba(49, 78, 104, 0.6) 2.08%, rgba(12, 17, 23, 0.6) 85.94%);
  }

  .filtre-green {
    position:absolute;
    top:0;
    left:0;
    width:100%;
    height:100%;
    background: linear-gradient(215.81deg, rgba(20, 52, 62, 0.38) 19.04%, rgba(37, 88, 99, 0.5) 34.07%, rgba(45, 126, 62, 0.48) 67.05%);
  }


</style>

<script>
  export default { 
    name : 'MainHero',
    data() {
      return {
        mainHero : 'main-hero',
        mainHeroAfter : 'main-hero-after'
      }
    },
    computed : {
      isRaptzPage() {
        if (this.hero.titre == undefined) {
            return  false ; 
        } else {
            return true ;
          }
      }
    },
    props : {
      hero : Object
    }
  }
</script>