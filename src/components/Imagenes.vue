<template>
  <section id="furgo-imagen">
      <div class="img-big"> 
          <img v-bind:src="fotos[0]" alt="Furgoneta Camper">
      </div>
        <div class="img-mini">
          <a @click="cambiarFoto(1)"><img  v-bind:src="fotos[1]" copyright="cc-by JuanManuel Añino" alt="Furgoneta Camper"></a>
          <a @click="cambiarFoto(2)"><img  v-bind:src="fotos[2]" copyright="cc-by JuanManuel Añino" alt="Furgoneta Camper"></a>
          <a @click="cambiarFoto(3)"><img  v-bind:src="fotos[3]" copyright="cc-by JuanManuel Añino" alt="Furgoneta Camper"></a>
          <a @click="cambiarFoto(4)"><img  v-bind:src="fotos[4]" copyright="cc-by JuanManuel Añino" alt="Furgoneta Camper"></a>
          <a @click="cambiarFoto(5)"><img  v-bind:src="fotos[5]" copyright="cc-by JuanManuel Añino" alt="Furgoneta Camper"></a>
        </div>
      </section>    
</template>

<script>
export default {
    Name: 'FurgoImagen',
    data () {
        return {
            fotos: [
                require ('../assets/1.jpg'),
                require ('../assets/1.jpg'),
                require ('../assets/2.jpg'),
                require ('../assets/3.jpg'),
                require ('../assets/4.jpg'),
                require ('../assets/5.jpg')]
        }
    },
    methods: {
        cambiarFoto(id) {
            this.fotos[0] = this.fotos[id]
        }
    }

}
</script>

<style escoped>
#furgo-imagen {
    border-radius: 25px;
    padding: 1rem;
    margin: 1rem;
    flex: 0 1 50%;
    width: 800px;

}

.img-big img{
    width: auto;
}

.img-mini {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
}
.img-mini img {
    width: 100px;
    border:2px solid #d8d8d8;
    
}
</style>