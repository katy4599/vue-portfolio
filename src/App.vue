<template>
  <div id="app">
   
      <!-- <nav>
      
        <router-link to="/" class="link">Home</router-link> |
        <router-link to="/resume" class="link">Resume</router-link>
      </nav> -->
    <router-view/>
  </div>
  
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #023047;
  height: 100%;
  background-color: #b1efe5;
  
}

// nav {
//   padding: 30px;
//   animation: fadeIn 0.5s ease-in 2s forwards;
//   background-color: #b1efe5;

//   a {
//     font-weight: bold;
//     color: #023047;

//     &.router-link-exact-active {
//       color: #90DBF4;
//     }
//   }
// }

// @keyframes fadeIn {
//   from { opacity: 0; }
//   to  { opacity: 1; }
// }

// .link {
//   z-index: 1;
// }

// .strip-top {
//   position: fixed;
//   width: 100%;
//   height: 12.5%;
//   top: 0;
//   background-color: #675CE0;
  
// }

// 

// 

</style>
