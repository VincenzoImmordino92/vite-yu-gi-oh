<script >
export default{
  name:'Header'
}

</script>

<template>
<header>
  <div class="image">
    <img src="/public/yu-gi-oh.jpeg" alt="">
  </div>
  <p>yu-gi-oh api</p>
</header>


</template>
  

<style lang="scss" scoped>

header{
  display: flex;
  align-items: center;
  height: 50px;
  background-color: white;
  .image{
    width: 15%;
    height:100%;
    img{
      height: 100%;
      object-fit: cover;
    }
  } 

  p{
    color: rgb(24, 28, 33);
    font-size: 2.3rem;
      margin: 0px 20px;
      text-transform: capitalize;
    }
}


</style>