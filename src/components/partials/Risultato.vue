<script >

import { store } from '../../data/store';

export default{
  name:'Risultato',
  computed:{
    outputResult(){
      if(store.oggettiList.length > 0){
        return 'Risultati trovati:' + store.oggettiList.length;
      }
      return 'Nessun  Risultato';
    }
  }
}

</script>

<template>
  <div class="box_cust">
    <p>{{ outputResult }}</p>
  </div>
  

 </template> 

<style lang="scss">

.box_cust{
  background-color: black;
  display: block;
  padding: 10px 0;
}



</style>