<template>
  <div>

    <HeaderComponent />

    <HeroSection />

    <MainComponent />

    <FooterComponent />

  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';
import HeroSection from './components/HeroSection.vue';

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
    HeroSection
}
}
</script>

<style lang="scss">

@import "./assets/style/global";
@import "./assets/style/var";
@import "./assets/style/utility";




</style>
