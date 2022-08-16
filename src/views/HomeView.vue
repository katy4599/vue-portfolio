<template>
  <div class="home" >
    
    <HelloWorld />
    <div class="fade-in">
      <router-link to="/" class="link">Home</router-link> |
      <router-link to="/resume" class="link">Resume</router-link>
      <div class="carouselCont">
        <agile class="carousel" :nav-buttons="true" :fade="true" :dots="true" :initial-slide="0" :slides-to-show="1" >
          <div class="slide" :index="0">
            <About id="about" @click="play" /> 
          </div>  
          <div class="slide" :index="1">
            <Experience id="experience" />
          </div>  
          <div class="slide" :index="2">
            <Project id="project" /> 
          </div> 
          <div class="slide" :index="3">
            <Project2 id="project2" /> 
          </div> 
          <div class="slide" :index="4">
            <h1 class="dogs">The Millard Team</h1>
            <h3 class="dogs">Gunner</h3>
            <h4 class="dogs">Chief of Security</h4>
            <img src="@/assets/Gunner.jpg" class="dogsGun" />
            <p class="dogAbout">Gunner has been a loyal member of the Millard team since 2018, when
              he graduated from Wayside Waifs. He contributes an immense amount of emotional support
              to the team leader. He has taken on the responsibility of orientating new team members and
              showing them which toys they are allowed to play with. Gunner regularly saves his team leader's
              life by loudly alerting her to every killer rabbit and attack squirrel that twitches, within a 
              two mile radius. Great Job Gunner!!!
            </p>
          </div> 
          <div class="slide" :index="5">
            <h1 class="dogs">The Millard Team</h1>
            <h3 class="dogs">Ranger</h3>
            <h4 class="dogs">Security Apprentice</h4>
            <img src="@/assets/Ranger.jpg" class="dogsRange" />
            <p class="dogAbout">Meet Ranger! He is the newest member of the team, joining us in June 2022,
              after ending his tenure with Unleashed Pet Rescue. He brings an abundant amount 
              of enthusiasm and is settling in well to his new role. He appreciates the mentorship
              he has received from his more experienced colleague. He is excited to expand his knowledge
              and skills. He is most excited to learn what "no" means, as is his human team leader. We look
              forward to seeing what toy Ranger murders next!!!
            </p>
          </div> 
          <div class="slide" :index="6">
            <Contact id="contact" /> 
          </div> 
          <template class="button" slot="prevButton">prev</template>
          <template class="button" slot="nextButton">next</template>
        </agile>
      </div>
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
import { VueAgile } from 'vue-agile'
import { computed } from 'vue'
// import { useSound } from '@vueuse/sound'
// import buttonSfx from '@/assets/SoundClip.mp3'

export default {
  // var myClip: new Audio(require('@/assets/SoundClip.mp3')),

  name: 'HomeView',
  components: {
    HelloWorld,
    agile: VueAgile,
    Carousel3d, 
    Slide,
    About,
    Contact,
    Experience,
    Project,
    Project2
  },
  props: [
    'width',
    'height',
    'border'
    ],
  computed: {
    slideHeight () {
    const sw = parseInt(this.width, 10) + (parseInt(this.border, 10) * 2)
    const sh = parseInt(parseInt(this.height) + (this.border * 2), 10)
    const ar = this.calculateAspectRatio(sw, sh)
    return this.slideWidth / ar
    }
  }
//   methods: {
//     playClip() {
//       myClip.play()
//     }
//   }
// }
}         
</script>

<style>

.home {
  position: fixed;
  height: 100%;
  width: 100%;
  background-color: #caf0f8;
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

.link {
  margin-top: 5%;
  color: #023047;
  text-decoration: none;
}

/* .carousel-3d-slide img {
    width: 40%;
    height: 40%;
} */

.carouselCont {
  width: 56%;
  margin-left: 22%;
  margin-right: 22%;
  height: 90% !important;
}

.carousel {
  width: 100%;
  height: 100%;
}
/* .carousel {
  padding-top: 15px;
  margin-bottom: 12.5%;
  /* margin-right: 20%;
  margin-left: 20%; */
  /* z-index: -1; */
  /* animation: fadeIn 3s;   */


.slide {
  background-position: center;
  background-size: cover;
  width: 100%;
  height: 100%;
  background-color: #5F97E0;
} 

.button {
  padding-top: 20px;
  background-color: #5F97E0 !important;
  font-family: Ubuntu, Helvetica, Arial, sans-serif;
}

.dogs {
  text-align: center;
  margin-bottom: 0px;
  margin-top: 2.5%;
}

.dogsGun {
  width: 25%;
  height: auto;
  padding-top: 2.5%;
  padding-bottom: 2.5%;
}

.dogsRange {
  width: 25%;
  height: auto;
  padding-top: 2.5%;
  padding-bottom: 2.5%;
}

.dogAbout {
  text-align: center !important;
  margin-left: 10% !important;
  margin-right: 10% !important;
  margin-top: 5px;
  width: 80% !important;
}

</style>
