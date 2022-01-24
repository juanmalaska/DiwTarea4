<template>
  <section>
    <div class="container">
      <nav>
        <ul class="breadcrumb">
          <li><a href="#">INICIO</a></li>
          <li><a href="#">RESERVAS</a></li>
          <li><a href="#">CAMPER</a></li>
        </ul>
      </nav>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
ul.breadcrumb {
  padding: 10px 16px;
  list-style: none;
  background-color: #eee;
}

ul.breadcrumb li {
  display: inline;
  font-size: 10px;
}

ul.breadcrumb li + li:before {
  padding: 8px;
  color: black;
  content: "/\00a0";
}

ul.breadcrumb li a {
  color: #0275d8;
  text-decoration: none;
}

ul.breadcrumb li a:hover {
  color: #01447e;
  text-decoration: underline;
}
</style>