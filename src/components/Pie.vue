<template>
  <footer class="pie">
    <div class="enlaces">
      <div class="izquierda">
       <p> <a href="#">Política de cookies</a></p>
       <p> <a href="#">Política de privacidad</a></p>
       <p> <a href="#">Condiciones generales</a></p>
      </div>
      
      <div class="cent">
       <p> <a href="#">Aviso legal</a></p>
       <p> <a href="#">Trabaja con nosotros</a></p>
       <p> <a href="#">¿Dónde estamos?</a></p>
      </div>
      <div class="loN">
      <img id="logon" alt="logotiponeg" src="@/assets/logoN.png" />
        </div>

  <div class="contc">   
<div class="redes">
  <div>
  <h3> ¡Síguenos!</h3>
  </div>
  <div class="red">
       <a href="#" id="face"><img id="f" alt="facebook" src="@/assets/face.png" /></a>
       
        <a href="#"  id="twitter"><img id="t" alt="twitter" src="@/assets/twitter.png" /></a>
         <a href="#"  id="instagram"><img id="i" alt="instagram" src="@/assets/insta.png" /></a>

         </div>
    </div>

    <div class="pagos">
  <div>
  <h3> Formas de pago</h3>
  </div>
  <div class="formap">
      <a href="#" id="credit"><img id="c" alt="facebook" src="@/assets/credit.png" /></a>
        <a href="#"  id="bizum"><img id="b" alt="twitter" src="@/assets/bizum.png" /></a>
         <a href="#"  id="pay"><img id="p" alt="instagram" src="@/assets/paypal.png" /></a>

         </div>
    </div>
    
   
      </div> 
      </div>
      
  </footer>
   <div class="copy">
      <p>&#169; 2022 Irina Casas Duarte</p>
    </div>
</template>

<script>
export default {};
</script>

<style>
.contc{

  display:flex;
  gap:10rem;
  margin-left:10rem;
}
.pie{
  display: flex;
  justify-content: space-between;
  background-color: #333333;
  margin-top:2rem;
  border-top-right-radius: 10px 10px;
 border-top-left-radius: 10px 10px;
}
.red{
 display:flex;
 gap:1.5rem;

 
}
.redes{
text-align: center;
  
  
  gap:2rem;
}
.pagos{

text-align: center;
 
}

.formap{
display:flex;

 gap:1.5rem;
}

 .redes h3{

    font-family: "Urbanist";
  color: rgb(223, 223, 223);
  
}

.pagos h3{
 font-family: "Urbanist";
  color: rgb(223, 223, 223);
  margin-left:-1rem;

}

#f{
  width: 2rem;
}
#t{
  width: 2rem;
}
#i{
  width: 2rem;
}
#c{
  width: 2.5rem;
}
#b{
  width: 2.5rem;
}
#p{
  width: 2.5rem;
}
#logon{
  width: 8rem;
  padding-top:2rem;
  padding-left:12rem;
}


.enlaces {
  display: flex; 

  border-top-left-radius: 10px 10px;
  border-top-right-radius: 10px 10px;
  align-items: center;
 
 padding-top:1.2rem;
  padding-bottom: 2rem;

  background-color: #333333;
}

.enlaces a {
  text-decoration: none;
  font-size: 1rem;
  font-weight: bolder;
 

  font-family: "Urbanist";
  color: rgb(223, 223, 223);
}

.izquierda {
  margin-left: 2rem;
  display: flex;
  margin-right:10rem;
  flex-direction: column;
  
 

}

.cent {
  display: flex;
  flex-direction: column;
 
  
}
</style>