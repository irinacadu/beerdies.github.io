<template>

  <section id="bread">
    <a class="inicio" href="#"> Inicio </a> 
    <a href="#"><span>/</span> Nuestras Cervezas </a>     
    <a class="actual" href="#"> <span>/</span> Craft Beer Culture</a>
  </section>
</template>

<script>
export default {};
</script>

<style>
#bread {
  display: flex;
  align-items: baseline;
  padding-top:1rem;
  padding-bottom: 2rem;
  
}

a {
  text-decoration: none;
font-family: "Carrois Gothic SC";
 
  color: black;
}

span{

font-weight: bolder;
  color:  #fe8a00;
}


</style>