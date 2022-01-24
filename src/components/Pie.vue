<template>
  <footer id="pie">
    <div class="contacto">
      <div>
        <figure>
          <img
            src="../assets/logo.png"
            copyright="cc-by-nc JuanManuel Añino"
            id="logo-pie"
          />
          <figcaption>
            Logo creado por Juan Manuel Añino
            <a href="https://creativecommons.org/licenses/by/2.0/">cc-by</a>
          </figcaption>
        </figure>
        <p>
          Alquiler de furgonetas camperizadas, perfectas para realizar, planear
          tu siguiente viaje.
        </p>
        <p>Que dices, ¿Te apuntas a una nueva aventura?</p>
      </div>
      <div>
        <h3>CONTACTO</h3>
        <p>
          Si tienes alguna duda, habla con nosotros por cualquiera de estas
          formas.
        </p>
        <p>666 555 444</p>
        <p>info@tucamper.com</p>
        <p>C/Murcia n*1 (Murcia)</p>
      </div>
      <div>
        <h3>REDES SOCIALES</h3>
        <p>
          Siguenos en rrss y descubre las experiencias de otros clientes y
          comparte las tuyas con nosotros.
        </p>
        <p>
          <img
            src="../assets/instagram.png"
            class="icono-redes"
            alt="Instagram tuCamper"
          />&nbsp;@tucamper
        </p>
        <p>
          <img
            src="../assets/twitter.png"
            class="icono-redes"
            alt="twitter tuCamper"
          />&nbsp; @tucamper
        </p>
        <p>
          <img
            src="../assets/facebook.png"
            class="icono-redes"
            alt="Facebook tuCamper"
          />&nbsp;tuCamper
        </p>
      </div>
    </div>
    <h5 id="derechos">© Copyright 2021 - Todos los derechos reservados</h5>
  </footer>
</template>

<script>
export default {};
</script>

<style>
#pie {
  background-color: #303030;
  padding-left: 20px;
  color: #fcfcfc;
}
#pie p {
  color: rgb(194, 194, 194);
  margin-left: 20px;
  margin-right: 20px;
}

#logo-pie {
  width: 200px;
}

.contacto {
  display: flex;
  flex-direction: row;
}

#derechos {
  align-items: center;
}

.icono-redes {
  width: 20px;
  height: 20px;
}
</style>