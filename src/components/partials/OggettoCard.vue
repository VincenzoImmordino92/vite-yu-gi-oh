<script >
export default{
  name:'OggettoCard',
  props:{
    name:String,
    archetype:String,
    image:String
  }
}

</script>

<template>
<div class="col-3 card_ctm">
  <img :src="image" :alt="name">
  <h4>{{ name }}</h4>
  <p>{{ archetype }}</p>
</div>

</template>

<style lang="scss">
@use '../../scss/partials/variabili' as*;

.card_ctm{
  text-align: center;
  margin-bottom: 10px;
  padding: px;
  border: 1px solid black;
  background-color: $primary-color;
  h4{
    color: white;
  }
  p{
    color: black;
  }
}


</style>