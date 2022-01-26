<template>
<center>
 <section id="producto-imagen">
      <div class="img-big"> 
          <img copyright="irinaC" id="principal" v-bind:src="fotos[0]" >
      </div>
      <center>
        <div class="miniaturas">
          <a @click="cambiarFoto(1)"><img copyright="irinaC" v-bind:src="fotos[1]" alt="Camden Town" title="Camden Town"></a>
         <a @click="cambiarFoto(2)"><img  copyright="irinaC" v-bind:src="fotos[2]" alt="Kaiju" title="Kaiju"></a>
          <a @click="cambiarFoto(3)"><img copyright="irinaC" v-bind:src="fotos[3]" alt="Cerveza Sagrada" title="Cerveza Sagrada"></a>
          <a @click="cambiarFoto(4)"><img copyright="irinaC" v-bind:src="fotos[4]" alt="Hacienda" title="Hacienda"></a>
        </div>
        </center>
      </section></center>

</template>


<script>
export default {

    Name: 'Imagenes',
    data(){
        return{
            fotos:[
                require('@/assets/Camden Town.jpg'),
                require('@/assets/Camden Town.jpg'),
                require('@/assets/Kaiju.jpg'),
                require('@/assets/Cerveza Sagrada.jpg'),
                require('@/assets/Hacienda.jpg')
            ]
        }
    },
    methods:{
        cambiarFoto(id){
            this.fotos[0]=this.fotos[id]
        }
    }
};
</script>

<style escoped>

#principal{

    width: 1500px;
}
.miniaturas img{
    margin-top:1rem;
     width: 244px;
     
     
}

.miniaturas {

    display:flex;
     
    
    gap:1rem;
   
    
}
#nombreIsla {
  color: white;
  font-family: "Urbanist";
  position: absolute;
  font-size: 5rem;
  font-weight: bolder;
  margin-top: -9rem;
  background-color: rgb(23, 32, 42, 0.45);

  padding-left: 2rem;
  padding-right: 2rem;
  padding-bottom: 0.5rem;
}
</style>