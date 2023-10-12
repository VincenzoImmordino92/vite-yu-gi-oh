<script >

import OggettoCard from './partials/OggettoCard.vue'
import Risultato from './partials/Risultato.vue'

export default{
  name:'ContainerCards',
  data(){
    return{

    }
  },
  components:{
    OggettoCard,
    Risultato
  }
}
</script>

<template>

<div class=" custom ">
  <Risultato />
  <div class="row">

  
  <OggettoCard />
  <OggettoCard />
  <OggettoCard />
  <OggettoCard />
  <OggettoCard />
  <OggettoCard />
  <OggettoCard />
  <OggettoCard />

  </div>

</div>



</template>

<style lang="scss">

.custom{
  background-color: white;
  margin: 0 auto;
  width: 100%;
  border: 1px solid black;
 
}


</style>