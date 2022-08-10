<template>
  <div class="resume">
    <nav class="resumeNav">
      
        <router-link to="/" class="link">Home</router-link> |
        <a href="/files/KatyMillard.pdf" download><btn class="link">Download Resume</btn></a>
        
    </nav>
    <img src="@/assets/Resume.png" class="resumeImg" />
  </div>
</template>

<script>

  export default {
    name: 'ResumeView',
    components: {
      
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
}

.resume {
  
  margin: 0px;
  padding: 0px;width: 100%;
  justify-items: center;
  /* position: fixed; */
  height: auto;
  background-color: #b1efe5;
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

  top: 5%;
}

.link {
  margin-top: 5%;
}

.resumeImg {
  margin-left: 15%;
  margin-right: 15%;
  margin-top: 10%;
  width: 70%;
  height: auto;
  border: 5px solid #675CE0;
  
}
</style>
