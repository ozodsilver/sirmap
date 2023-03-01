<template>
    <div>
        <nav>
        <div class="container">
            <div class="logo">
                <img src="../assets/logo.png" alt="">
                <h4 class="text1">Age<h4 class="text2">Syrdarya</h4></h4>
             </div>

             <ul class="linkbox">
                <li class="link1 link">Loyiha haqida</li>
                <li class="link2 link">Infografika</li>
                <li class="link3 link">Biz bilan bog’lanish</li>
             </ul>

             <button class="knopka">Uzb <i class="fas fa-angle-down"></i></button>



<div class="icons">
    <i class="fab fa-instagram fa-2x"></i>
    <i class="fab fa-facebook-f fa-2x"></i>
</div>

        </div>
        </nav>
    </div>
</template>

// css qismi

<style>
  nav{
    width: 100%;
    height: 7vh;
    background-color: #01094F ;
    display: flex;

  }
  .container{
    display: flex;
    align-items: center;

  }
  .logo{
    width: 20%;
    height: 7vh;
    display: flex;
    align-items: center;
  }
  .text1{
    display: inline-block;
    color: #FFE500;
    margin-top: 10px;
  }
  .text2{
    display: inline-block;
    color: white;
    margin-top: 10px;
  }
  .linkbox{
    display: flex;
    color: white;
    list-style: none;
    margin-left: 300px;
    margin-top: 13px;
  }
  .link{
   margin: 10px;
  }
  .knopka{
    border: none;
    background-color: #01094F;
    color: white;
    margin-left: 20px;
  }
  .icons{
    width: 10%;
    color: white;
    display: flex;
    justify-content: space-evenly;
  }

</style>



// script qismi

<script>

</script>