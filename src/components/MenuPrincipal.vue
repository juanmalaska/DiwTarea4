<template>
<section id="menu-principal">
    <div class="container">
    <nav>
        <ul>
            <li><a href="#">INICIO</a></li>
            <li><a href="#">RESERVAS</a></li>
            <li><a href="#">NOSOTROS</a></li>
            <li><a href="#">CAMPERIZACIONES</a></li>
            <li><a href="#">FURGONETAS</a></li>
            <li><a href="#">AUTOCARAVANAS</a></li>
        </ul>
    </nav>
</div>
</section>
  
</template>

<script>
export default {

}
</script>

<style>
section#menu-principal {
    background: #1abc9c;
    z-index:999;
    padding:0.7rem;
}

section#menu-principal .container {
    display: flex;
    justify-content: space-between;
}

section#menu-principal .container nav ul {
    display:flex;
    list-style: none;
    padding: 0;
    margin:0rem 0.7rem;
}
section#menu-principal .container nav ul li a{
    background-color: #1abc9c;
    text-decoration: none;
    color:white;
    font-weight: 700;
    padding-left: 1rem;
    padding-right: 1rem;
}
section#menu-principal .container nav ul li a:hover,.active{
    text-decoration: none;
    color:white;
    font-weight: 700;
    padding: 1rem;
}


</style>