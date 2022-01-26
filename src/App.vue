<template class="general">
  <div>
    <Cab />
  </div>
  <div>
    <Bread />
  </div>

  <div class="fot">
    <Imagenes />
  </div>
  <div class="central">
    
      <Descripcion />
    

    <div>
      <Video />
    </div>
  </div>
  <div>
    <birras />
  </div>

  <div class="foot">
    <Pie />
  </div>
</template>

<script>
import Cab from "./components/Cab.vue";
import Bread from "./components/Bread.vue";
import Imagenes from "./components/Imagenes.vue";
import Descripcion from "./components/Descripcion.vue";
import Video from "./components/Video.vue";
import birras from "./components/birras.vue";
import Pie from "./components/Pie.vue";

export default {
  name: "App",
  components: {
    Cab,
    Bread,
    Imagenes,
    Descripcion,
    Video,
    birras,
    Pie,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Carrois+Gothic+SC&family=Monoton&family=Petit+Formal+Script&family=Urbanist:wght@300&display=swap");
#nEmpre {
  text-align: center;
}

body {
  width: 1500px;
  margin-left: auto;
  margin-right: auto;
  background-color: #fffcfa;
}

.central {
  display:flex;

  
  
}
.general {
  display: flex;
  flex-direction: column;
}
</style>