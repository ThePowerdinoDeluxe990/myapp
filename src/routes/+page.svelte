<svelte:head>
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-9ndCyUaIbzAi2FUVXJi0CjmCapSmO7SnpJef0486qhLnuZ2cdeRhO02iuK6FUUVM" crossorigin="anonymous">
</svelte:head>

<script lang="ts">
let index:number = 1;

</script>

<div id="menu" class="bg-dark sticky-top">
    <h1 id="title" >Menú Pizzeria</h1>
        <p id="1" on:click|preventDefault={()=>(index=1)} class="text-center ">Pizzas</p>
        <p id="2" on:click|preventDefault={()=>(index=2)} class="text-center ">Bebidas</p>
        <p id="3" on:click|preventDefault={()=>(index=3)} class="text-center ">Entrantes</p>
        <p id="4" on:click|preventDefault={()=>(index=4)} class="text-center ">Postres</p>
</div>


{#if index===1}
<div class="mx-auto text-center bg-secondary w-50">
   
    <h1 class="text-white">Pizza Margarita</h1>
    <img src="https://www.annarecetasfaciles.com/files/pizza-margarita-1-scaled.jpg">
 
    <h1 class="text-white">Pizza Pepperoni</h1>
    <img src="https://images.hola.com/imagenes/cocina/recetas/20220208204252/pizza-pepperoni-mozzarella/1-48-890/pepperoni-pizza-abob-m.jpg">

    <h1 class="text-white">Pizza Carbonara</h1>
    <img src="https://cocinaabuenashoras.com/files/pizza-carbonara-1-815.jpeg">

    <h1 class="text-white">Pizza Calzone</h1>
    <img src="https://okdiario.com/img/recetas/2017/07/12/pizza-calzone-3.jpg">
   
</div>
{:else if index===2}

<div class="mx-auto text-center bg-secondary w-50">
   
    <h1 class="text-white">Fanta</h1>
    <img src="https://www.pngplay.com/wp-content/uploads/12/Fanta-PNG-Photo-Image.png">
 
    <h1 class="text-white">Pepsi</h1>
    <img src="https://www.pngplay.com/wp-content/uploads/1/Pepsi-PNG-Free-Image.png">

    <h1 class="text-white">Coca Cola</h1>
    <img src="https://www.pngall.com/wp-content/uploads/2016/04/Coca-Cola-PNG-Picture.png">

    <h1 class="text-white">Nestea</h1>
    <img src="https://www.fornoantico.es/35-medium_default/nestea-limon.jpg">
   
</div>

{:else if index ===3}

<div class="mx-auto text-center bg-secondary w-50">
   
    <h1 class="text-white">Caprese</h1>
    <img src="https://estag.fimagenes.com/imagenesred/2569414_0.jpg?1">
 
    <h1 class="text-white">Sticks de mozzarella</h1>
    <img src="https://i.ytimg.com/vi/BBwKKFFShII/maxresdefault.jpg">

    <h1 class="text-white">Panecillos de Ajo</h1>
    <img src="https://i.ytimg.com/vi/YHhQLlU-VnQ/maxresdefault.jpg">

    <h1 class="text-white">Patatas Bravas</h1>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/16/Patatas_bravas_madrid.jpg/640px-Patatas_bravas_madrid.jpg">
   
</div>

{:else if index ===4}
<div class="mx-auto text-center bg-secondary w-50">
   
    <h1 class="text-white">Helado </h1>
    <h4>Sabores:</h4>

    <h6 class="text-warning">·Fresa,Vainilla,Chocolate,Café</h6>
    <img src="https://images.hola.com/imagenes/cocina/noticiaslibros/20230412229842/helados-sabores-originales-recetas/1-233-402/helados-varios-adob-t.jpg">
 
    <h1 class="text-white">Tiramisú</h1>
    <img src="https://vdmedia.elpais.com/elpaistop/20183/23/201803232226750_1521841141_asset_still.png">

    <h1 class="text-white">Brownie</h1>
    <img src="https://img2.rtve.es/imagenes/aqui-tierra-receta-brownie-jesus-monedero/1585576217689.JPG">

    <h1 class="text-white">Natillas</h1>
    <img src="https://img2.rtve.es/i/?w=1600&i=1619780561856.jpg">
   
</div>

{/if}

<style>
    img{
        max-width: 500px;
        max-height: 500px;
        padding-bottom:50px;
    }p{
        color:aliceblue;
        padding-left:30px;
    }
    #menu{
        padding:0px;
       
    }
    #menu p{
        display: inline;
        padding-top:0px;
    }
    p:hover{
        cursor: pointer;
        color:aquamarine;
    }
    p:active{
        color:red;
    }
    #title{
        padding-left:20px;
        font-size: large;
        color:aliceblue;
    }
</style>
