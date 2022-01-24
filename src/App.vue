<template>

<div class="top">
  
  <Buscador/>
  <InicioSesion/>
</div>

<div id="menu">
<Cabe/>
<MenuPrincipal/>
</div>

<div>
  <Bread/>
</div>

<div class="fotos-reserva">
  <div id="principal">
    <Imagenes/>
  </div>
  <div>
    <Informacion/>
  </div>
</div>

<div class="container">
   <Descripcion/>
  </div>
  
<div>
<Pie/>
</div>

</template>

<script>
import Cabe from './components/Cabe.vue'
import Buscador from './components/Busca.vue'
import Pie from './components/Pie.vue'
import InicioSesion from './components/InicioSesion.vue'
import MenuPrincipal from './components/MenuPrincipal.vue'
import Bread from './components/Bread.vue'
import Imagenes from './components/Imagenes.vue'
import Informacion from './components/Informacion.vue'
import Descripcion from './components/Descripcion.vue'


export default {
  name: 'App',
  components: {
    Cabe,
    Buscador,
    InicioSesion,
    MenuPrincipal,
    Bread,
    Imagenes,
    Informacion,
    Descripcion,
    Pie
  }
}
</script>

<style>

body{
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}

.top{
  display: flex;
  flex-flow: row;
  align-items: center;
  justify-content: flex-end;
  border-bottom: 1px solid black;
}

#menu{
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}

.fotos-reserva{
  display: flex;
  flex-direction: row;
  padding-right: 120px;
}
#principal{
  flex-grow: 0;
  width: auto;
  padding-left: 80px;
}

#app {
  font-family: 'Titillium Web', sans-serif;
}
</style>

