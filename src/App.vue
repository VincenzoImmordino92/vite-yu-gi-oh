<script >
import axios from 'axios';
import Header from './components/Header.vue';
import ContainerCards from './components/ContainerCards.vue';
import Select from './components/partials/Select.vue';
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
    Select
    
  },
  methods:{
    getApi(){
      axios.get(store.apiUrl)
        .then(res =>{
          store.oggettiList = res.data.data
          store.immaginiList = res.data.data

          console.log(store.oggettiList);
          console.log(store.immaginiList);
        })
        .catch(err =>{
          console.log(err);
        })
    }
  },
  mounted(){
    this.getApi()
  }
}

</script>

<template>

  <Header />
  <Select />
  <ContainerCards />

</template> 

<style lang="scss">

@use './scss/main.scss'


</style>
