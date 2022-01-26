<template class="cervezas">
  <div class="iServ">
    <h2 id="idisp">Elige tus Birras</h2>
  </div>

  <div class="birras">
    <div class="camden">
      <h3>CAMDEN TOWN</h3>
      <p>20 €/pack de 4 (330ml)</p>
      <div class="cont1">
        <div>
          <button
            class="btn"
            @click="cambiarContador('-1')"
            type="button"
            name="button"
          >
            -
          </button>
          <input class="cantidad" type="text" name="name" :value="contador" />
          <button
            class="btn"
            @click="cambiarContador('1')"
            type="button"
            name="button"
          >
            +
          </button>
        </div>
      </div>
      <button id="saca" type="button">¡Al carrito!</button>
    </div>
    <div class="sagrada">
      <h3>CERVEZA SAGRADA</h3>
      <p>18 €/pack de 3 (330ml)</p>
      <div class="contado">
        <button class="btn" @click="cambiarC('-1')" type="button" name="button">
          -
        </button>
        <input class="cantidad" type="text" name="name" :value="contado" />
        <button class="btn" @click="cambiarC('1')" type="button" name="button">
          +
        </button>
      </div>
      <div class="saca1">
      <button id="saca" type="button">¡Al carrito!</button>
      </div>
    </div>

    <div class="kaiju">
      <h3>KAIJU!</h3>
      <p>15 €/pack de 3 (330ml)</p>
      <div class="cont">
        <button class="btn" @click="cCont('-1')" type="button" name="button">
          -
        </button>
        <input class="cantidad" type="text" name="name" :value="cont" />
        <button class="btn" @click="cCont('1')" type="button" name="button">
          +
        </button>
      </div>
      <div class="saca2">
      <button id="saca" type="button">¡Al carrito!</button>
      </div>
    </div>
  </div>

  <div class="hacienda">
    <h3>HACIENDA</h3>
    <p>25 €/pack de 3 (330ml)</p>
    <div class="contar">
      <button class="btn" @click="cambiar('-1')" type="button" name="button">
        -
      </button>
      <input class="cantidad" type="text" name="name" :value="contar" />
      <button class="btn" @click="cambiar('1')" type="button" name="button">
        +
      </button>
    </div>
    <div class="saca4">
    <button id="saca" type="button">¡Al carrito!</button>
    </div>
  </div>
 
</template>

<script>
export default {
  Name: "ProductoDatos",
  data() {
    return {
      contador: 1,
      contar: 1,
      contado: 1,
      cont: 1,
    };
  },
  methods: {
    cambiarContador(num) {
      this.contador += +num;

      if (!isNaN(this.contador) && this.contador < 0) {
        this.contador = 0;
      }
    },
    cambiar(num) {
      this.contar += +num;
      if (!isNaN(this.contar) && this.contar < 0) {
        this.contar = 0;
      }
    },
    cCont(num) {
      this.cont += +num;
      if (!isNaN(this.cont) && this.cont < 0) {
        this.cont = 0;
      }
    },
    cambiarC(num) {
      this.contado += +num;
      if (!isNaN(this.contado) && this.contado < 0) {
        this.contado = 0;
      }
    },
  },
};
</script>

<style>

.iServ{
  margin-top:-1rem;
}
h3{
  font-family: "Urbanist";
  font-size:1.5rem;
  
}

p{

  font-family: "Urbanist";
}
.camden {
  display: flex;
  align-items: baseline;
  
  border-bottom: rgb(179, 176, 176) solid thin;
  gap:15rem;
}

.camden p{

  padding-left:10rem;
}

.sagrada {
  display: flex;
  align-items: baseline;
  border-bottom: rgb(179, 176, 176) solid thin;
  gap:14.5rem;
}

.sagrada p{

  margin-left: 7.5rem;
}
.contado{

  margin-left: 0.9rem;
}
.saca1{
  margin-left:0.6rem;
}

.kaiju {
  display: flex;
  align-items: baseline;
    border-bottom: rgb(179, 176, 176) solid thin;
  gap:15rem;
}

.kaiju p{
  margin-left:16.7rem;
}
.cont{
  margin-left:0.4rem;
}
.saca2{
  margin-left:0.3rem;
}
.hacienda {
  display: flex;
  align-items: baseline;
    border-bottom: rgb(179, 176, 176) solid thin;
  gap:15rem;
}
.hacienda p{

  margin-left:13.4rem;
}

.contar{

  margin-left:0.3rem;
}

.saca4{
  margin-left:0.3rem;
}
.contador {
  display: flex;
  align-items: baseline;

  padding-left: 2.7rem;
  margin-top: 2rem;
}

.btn {
  font-family: "Urbanist";
  background-color: #fe8a00;
  width: 2rem;
  height: 2rem;
  color: white;
  border-radius: 10rem;
  align-self: center;
}

.cantidad {
  width: 2rem;
  text-align: center;
  border-radius: 10rem;
  height: 2rem;
  font-size: 1rem;
  font-family: "Urbanist";
}

#idisp {
  color: #8f8f8f;
  font-size: 2rem;
  font-family: "Carrois Gothic SC";
  border-bottom: #8f8f8f solid thin;
}

#saca {
  font-family: "Urbanist";
  font-size: 1rem;

  background-color: #999897;
  width: 10rem;
  height: 2rem;
  text-align: center;
  border-radius: 0.5rem;
  color: white;

  margin-top: 2rem;
}

#saca:hover {
  background-color: #fe8a00;
  color: white;
  font-weight: bolder;
  border-radius: 5rem;
}
</style>