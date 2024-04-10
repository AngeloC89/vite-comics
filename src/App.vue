<template>
  <div>
<HeaderComponent/>
<JumpoTron/>
<MainComponent/>
<FooterComponent/>
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import JumpoTron from './components/JumpoTron.vue';
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';



  export default {
    name:'App',
    components: {
      HeaderComponent,
      JumpoTron,
      MainComponent,
      FooterComponent,
    },
    
  }
</script>

<style lang="scss" scoped>

</style>



