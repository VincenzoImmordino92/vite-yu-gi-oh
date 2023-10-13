<script >

import OggettoCard from './partials/OggettoCard.vue'
import Risultato from './partials/Risultato.vue'
import { store } from '../data/store';


export default{
  name:'ContainerCards',
  data(){
    return{
      store
    }
  },
  components:{
    OggettoCard,
    Risultato
  }
}
</script>

<template>

<div class="container custom">
  <Risultato />
  <div class="row">

  
  <OggettoCard v-for="card in store.oggettiList" 
                :key="card.id"
                :name="card.name"
                :archetype="card.archetype"
                :image="card.card_images[0].image_url_small"
              />
  

  </div>

</div>



</template>

<style lang="scss">

.custom{
  background-color: white;
  margin: 0 auto;
  width: 100%;
  margin: 30px;
  border: 1px solid black;
 
}


</style>