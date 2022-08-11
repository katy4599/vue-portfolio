<template>
    <div class="container w50 center tiny-w50" @click="play" >
        <header class="txtcenter mt2">
            <img  class="katy" src="@/assets/Katy.Millard.png"  alt="Avatar" />
            <h1>Katy Millard</h1>
            <h2 class="ma0">Junior Software Developer</h2>
            <h4>Kansas City, Missouri</h4>
        </header>
    
        <section class="mt3 mb3 pa1">
            <p class="bigger">
            And if you threw a party - invited everyone you knew. You would see the biggest gift would be from me and the card attached would say thank you for being a friend! 
            </p>
        </section>
    </div>
    
      
      

      

   
  

</template>

<script>
import { useSound } from '@vueuse/sound'
import buttonSfx from '../assets/SoundClip.mp3'

export default {
  name: 'About',
  props: {
    },
  setup() {
    const { play, stop } = useSound(buttonSfx)
      return {
        play,
        stop
      }
  },
}

</script>

<style>

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
  font-family: 'Merriweather', serif;
  margin-top: 7px;
  text-align: center;
}

section {
  font-family: 'Merriweather Sans', serif;
  text-align: center;
  font-size: .8em;
  color: #023047;
  width: 80%;
  margin-left: 10%;
  
}

</style>