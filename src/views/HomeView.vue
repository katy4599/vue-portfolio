<template>
  <div class="home" >
    
    <HelloWorld />
    <div class="fade-in">
      <router-link to="/" class="link">Home</router-link> |
      <router-link to="/resume" class="link">Resume</router-link>
      <carousel-3d class="carousel" :perspective="180" :controlsWidth="20" :controls-visible="true" :width="530" :height="490" :display="1">
        <slide class="slide" :index="0">
          <About id="about" /> 
        </slide> 
        <slide class="slide" :index="1">
          <Knowledge id="knowledge" />
        </slide>  
        <slide class="slide" :index="2">
          <Experience id="experience" />
        </slide>  
        <slide class="slide" :index="3">
          <Contact id="contact" /> 
        </slide> 
      </carousel-3d>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

// import "swiper/css/effect-flip";
// import "swiper/css/pagination";
// import "swiper/css/navigation";



// import required modules
// import {  Navigation } from "swiper";


import HelloWorld from '@/components/HelloWorld.vue'
import About from '@/components/About.vue'
import Knowledge from '@/components/Knowledge.vue'
import Experience from '@/components/Experience.vue'
import Contact from '@/components/Contact.vue'
import { Carousel3d, Slide } from 'vue-carousel-3d';








export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    Carousel3d, 
    Slide,
    About,
    Experience,
    Contact,
    Knowledge
  }
  
  
}
        
  
</script>

<style>



.home {
  position: fixed;
  height: 100%;
  width: 100%;
  background-color: #b1efe5;
  top: 0px;
  bottom: 0px;
}

.fade-in {
   animation: fadeIn 3s;  
   padding-top: 15px;
}

  @keyframes fadeIn {
  0% { opacity: 0; }
  10% { opacity: 0.005; }
  50% { opacity: 0.01; }
  100% { opacity: 1; }
}  

.carousel {
  padding-top: 15px;
  margin-bottom: 12.5%;
  margin-right: 20%;
  margin-left: 20%;
  z-index: -1;
  /* animation: fadeIn 3s;   */
}

  /* @keyframes fadeIn {
  0% { opacity: 0; }
  10% { opacity: 0.005; }
  50% { opacity: 0.01; }
  100% { opacity: 1; }
} */


.carousel-3d-slide img {
    width: 40%;
}


.slide {
  background-position: center;
  background-size: cover;
  width: 600px;
  height: auto;
  background-color: #5DC5D8;
} 








</style>
