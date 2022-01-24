<template>
  <section id="producto-datos">
      <h1>Sprinter maite-activity</h1>
      <h1>99€ <span class="iva"> /noche</span></h1>

      <div>
        <ul>
            <li>
              <span>Fecha Inicio:&nbsp; </span>
              <input type="date" name="start" value="" data-value="19-01-2022">

            </li>
          </ul>
      </div>
      <div class="wrapper">
        <ul>
            <li>
              <span class="iva">Numero de noches: &nbsp;</span>
            </li>
        </ul> 
          <button class="btn" @click="cambiarContador('-1')" type="button" name="button">-</button>
          <input class="cantidad" type="text" name="name" :value="contador">
          <button class="btn" @click="cambiarContador('1')" type="button" name="button">+</button>
        
      </div>
      <br>
      <button class="boton">RESERVAR</button>
  </section>
</template>

<script>
export default {
  Name: 'ProductoDatos',
    data () {
        return {
            contador: 1
        }
    },
    methods: {
        cambiarContador(num) {
            this.contador += +num;
            if (!isNaN(this.contador) && (this.contador < 0)) {
              this.contador = 0
            }
        }
    }


}
</script>

<style>
section#producto-datos {
  flex: 1 1 18rem;
}
h1 {
  font-size: 2.2rem;
}
h2 {
  font-size:1.7rem;
  color: #1abc9c;
}
span.iva {
  font-size:1rem;
  font-weight: normal;
  color: #282828
}
.wrapper {
  height: 2rem;
  display: flex;
}

.cantidad {
  border: none;
  text-align: center;
  width: 2rem;
  font-size: 1.2rem;
  border: 1px solid #d8d8d8;
}
.btn {
  border: 1px solid #d8d8d8;
  width: 1.8rem;
}
.boton{
    background-color: #1abc9c;
    text-decoration: none;
    color:white;
    font-weight: 700;
    padding: 1rem;
}
</style>