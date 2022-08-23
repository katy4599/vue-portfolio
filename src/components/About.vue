<template>
    <div class="container w50 center tiny-w50" >
        <header class="txtcenter mt2">
            <img  class="katy" src="@/assets/KatyHead.jpg"  alt="Avatar" />
            <h1>Katy Millard</h1>
            <h2 class="ma0">Junior Software Developer</h2>
            <h4>Kansas City, Missouri</h4>
        </header>
    
        <section class="mt3 mb3 pa1">
            <p class="bigger">
            I am a highly-motivated IT professional with expertise across several platforms,
            including full-stack development, implementation, and UI/UX design. I am a life long
            Kansas Citian who actually enjoys our Winter weather!
            </p>
        </section>
    </div>
    
      
      

      

   
  

</template>

<script>


export default {
  name: 'About',
  props: {
    },
  
}

</script>

<style scoped>

.container {
  opacity: 1;
  z-index: 1;
  /* animation: fadeIn 0.5s  */
}

/* @keyframes fadeIn {
  from { opacity: 0; }
  to  { opacity: 1; }
} */
.carousel-3d-slide img {
    width: 40%;
}
.katy {
  border-radius: 50%;
  border: 5px solid #5DC5D8;
  background-color: #5DDFD0;
  width: 200px;
  height: 200px;
  
}

header {
  font-family: Ubuntu, Helvetica, Arial, sans-serif;
  margin-top: 2.5%;
  text-align: center;
}

section {
  font-family: Ubuntu, Helvetica, Arial, sans-serif;
  text-align: center;
  font-size: .8em;
  color: #023047;
  width: 70%;
  margin-left: 15%;
  
}

</style>