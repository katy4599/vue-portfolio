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
          <Experience id="experience" />
        </slide>  
        <slide class="slide" :index="2">
          <Project id="project" /> 
        </slide> 
        <slide class="slide" :index="3">
          <Project2 id="project2" /> 
        </slide> 
        <slide class="slide" :index="4">
          <h1 class="dogs">The Millard Team</h1>
          <h3 class="dogs">Gunner</h3>
          <img src="@/assets/Gunner.jpg" class="dogsGun" />
          <p class="dogAbout">Gunner has been a loyal member of the Millard team since 2018, when
            he graduated from Wayside Waifs. He contributes an immense amount of emotional support
            to the team leader. He has taken on the responsibility of orientating new team members and
            showing them which toys they are allowed to play with. Gunner regularly saves his team leader's
            life by loudly alerting her to every killer rabbit and attack squirrel that twitches, within a 
            two mile radius. Great Job Gunner!!!
          </p>
        </slide> 
        <slide class="slide" :index="5">
          <h1 class="dogs">The Millard Team</h1>
          <h3 class="dogs">Ranger</h3>
          <img src="@/assets/Ranger.jpg" class="dogsRange" />
          <p class="dogAbout">Meet Ranger! He is the newest member of the team, joining us in June 2022,
            after ending his tenure with Unleashed Pet Rescue. He brings an abundant amount 
            of enthusiasm and is settling in well to his new role. He appreciates the mentorship
            he has received from his more experienced colleague. He is excited to expand his knowledge
            and skills. He is most excited to learn what "no" means, as is his human team leader. We look
            forward to seeing what toy Ranger murders next!!!
          </p>
        </slide> 
        <slide class="slide" :index="6">
          <Contact id="contact" /> 
        </slide> 
      </carousel-3d>
    </div>
  </div>
</template>

<script>

import HelloWorld from '@/components/HelloWorld.vue'
import About from '@/components/About.vue'
import Experience from '@/components/Experience.vue'
import Contact from '@/components/Contact.vue'
import Project from '@/components/Project.vue'
import Project2 from '@/components/Project2.vue'
import { Carousel3d, Slide } from 'vue-carousel-3d';

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    Carousel3d, 
    Slide,
    About,
    Contact,
    Experience,
    Project,
    Project2
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

.carousel-3d-slide img {
    width: 40%;
    height: 40%;
}

.carousel {
  padding-top: 15px;
  margin-bottom: 12.5%;
  margin-right: 20%;
  margin-left: 20%;
  z-index: -1;
  /* animation: fadeIn 3s;   */
}

.slide {
  background-position: center;
  background-size: cover;
  width: 600px;
  height: auto;
  background-color: #5DC5D8;
} 

.dogs {
  text-align: center;
  margin-bottom: 0px;
  margin-top: 10px;
}

.dogsGun {
  width: 200px !important;
  height: 200px !important;
  padding-left: 30% !important;
  padding-top: 10px;
}

.dogsRange {
  width: 200px !important;
  height: 200px !important;
  padding-left: 30% !important;
  padding-top: 10px;
}

.dogAbout {
  text-align: center !important;
  margin-left: 10% !important;
  margin-right: 10% !important;
  margin-top: 5px;
  width: 80% !important;
}

</style>
