<script >
export default{
  name:'OggettoCard'
}

</script>

<template>
<div class="col-3 card_ctm">
  <img src="#" alt="card">
  <h4>title</h4>
  <p>specie</p>
</div>

  </template>

<style lang="scss">
@use '../../scss/partials/variabili' as*;

.card_ctm{
  text-align: center;
  margin-bottom: 10px;
  padding: 20px;
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