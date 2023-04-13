<template>
  <HeaderComponent />
  <MainComponent />
  <MainBottom />
  <TopFooter />
  <BottomFooter />
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import MainBottom from './components/MainBottom.vue';
import TopFooter from './components/TopFooter.vue';
import BottomFooter from './components/BottomFooter.vue';
  export default {
    name: 'App',
    components: {
      HeaderComponent,
      MainComponent,
      MainBottom,
      TopFooter,
      BottomFooter
    }
  }
</script>

<style lang="scss" scoped>

</style>