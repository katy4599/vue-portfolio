<template>
  <div id="app">
   
      <!-- <nav>
      
        <router-link to="/" class="link">Home</router-link> |
        <router-link to="/resume" class="link">Resume</router-link>
      </nav> -->
    <router-view/>
  </div>
  
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Ubuntu&display=swap');

</style>

<style lang="scss">
#app {
  font-family: Ubuntu, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #023047;
  height: 100%;
  background-color: #b1efe5;
  
}

</style>
