<script >

import Header from './components/Header.vue';
import ContainerCards from './components/ContainerCards.vue';
import { store } from './data/store';

export default{
  name:'App',
  data(){
    return{
      store
    }
  },
  components:{
    Header,
    ContainerCards,
    
  }
}

</script>

<template>

  <Header />
  <ContainerCards />

</template> 

<style lang="scss">

@use './scss/main.scss'


</style>
