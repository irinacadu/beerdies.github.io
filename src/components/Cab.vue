<template>
<center>
  <header class="cab">
    

    <img id="logo" alt="logotipo" src="@/assets/mrBeer.png" />

   <h2 id="beerdies">BEERDIES</h2>

    <div class="centroCab">
      <select id="menu">
        <option value="pacifico">Nuestras Cervezas</option>
        <option value="pacifico">IPA</option>
        <option value="atlantico">Lager</option>
        <option value="indico">Negras</option>
        <option value="indico">Craft Beer Culture</option>
      </select>

      <a href="#"> ¿Quiénes somos?</a>
    
       <a href="#">¡Contacta!</a>
    </div>
    <div class="botones">
      <button id="b1" type="button" value="Mi cuenta">Mi cuenta</button>
      <button id="b2" type="button" value="Crear cuenta">Crear Cuenta</button>
    </div>


   <button class="icono"><i id="basket" class="fa fa-shopping-basket" aria-hidden="true" ></i></button>


  </header>
  </center>
</template>

<script>
export default {};
</script>

<style>

.icono{

  width: 2.5rem;
  height: 2.5rem;
  border-radius: 5rem;
  background-color:  #fe8a00;
  color:white;
}
.icono:hover{

  background-color: yellowgreen;
}


.centroCab {
  display: flex;
  align-items: center;
 margin-left: 16rem;
  font-size:1rem;
 gap:5rem;
}

#beerdies {
  font-family: "Carrois Gothic SC";
  color:  #fe8a00;
}
.botones {
  display: flex;
  align-items: flex-end;
  gap: 1.5rem;
  margin-left: 10rem;
  padding-right: 2rem;
}
#b1,
#b2 {
  font-family: "Urbanist";
  font-size: 1rem;
  background-color: white;
  width: 8rem;
  text-align: center;
}
#b1:hover, #b2:hover{

  background-color:  #fe8a00;
color:white;
font-weight: bolder;
border-radius: 5rem;
}

.centroCab a {
  text-decoration: none;
  color: black;
  font-family: "Urbanist";
  font-size: 1rem;

}
.cab {
  display: flex;
  align-items: center;

  
  border-bottom: #3d3c3b solid thin;
  
}
#menu {
  width: 12rem;
  font-family: "Urbanist";
  font-size: 1rem;
  background-color: white;
  text-align: center;
}

#logo {
  width: 6rem;
}




</style>