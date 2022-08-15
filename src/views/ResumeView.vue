<template>
  <div class="resume">
    <img src="@/assets/Resume.png" class="resumeImg" />
    <VueScrollFixedNavbar :isFixed="true" class="resumeNav">
      <nav class="link" >
        
          <router-link to="/" class="link">Home</router-link> |
          <a href="/files/KatyMillard.pdf" class="link" download><btn>Download Resume</btn></a>
          
      </nav>
    </VueScrollFixedNavbar>
  </div>
</template>

<script>
  import {VueScrollFixedNavbar} from "vue-scroll-fixed-navbar";

  export default {
    name: 'ResumeView',
    components: {
      VueScrollFixedNavbar
    }
  }
</script>

<style>

html {
  margin: 0px;
  padding: 0px;
  width: 100%;
  height: 100%;
  background-color: #b1efe5;
  top: 0px;
  bottom: 0px;
  left: 0px;
  right: 0px;
  font-family: Ubuntu, Helvetica, Arial, sans-serif;
}

.resume {
  
  margin: 0px;
  padding: 0px;width: 100%;
  justify-items: center;
  /* position: fixed; */
  height: auto;
  background-color: #caf0f8;
  background-size: cover;
  top: 0px;
  bottom: 0px;
  left: 0px;
}

.resumeNav {
  text-align: center;
  width: 100%;
  position: fixed;
  height: 12.5%;
  background-color: #5F97E0;
  top: 0;
  left: 0;
}

.link {
  margin-top: 2% !important;
  color: #023047;
  text-decoration: none;
}

.resumeImg {
  margin-left: 15%;
  margin-right: 15%;
  margin-top: 10%;
  width: 70%;
  height: auto;
  border: 5px solid #5F97E0;
  z-index: 1;
}
</style>
