<template>
    <div class="project">
      <h1>Featured Projects!</h1>
      <div class="temp-convert">
        <h3>Temperature Converter</h3>
        <img class="projectImg" src="@/assets/TempConvert.png" />
        <p class="desc">This JavaScript project was completed as an apprentice at SnapIT.
             It converts between four units of temperature. The background 
             picture changes depending on the comfort level of the resulting
             temperature. </p>
        <a :href="tempConvertUrl">
            <p>Try it Live!!!</p>
        </a>  
      </div>
    </div>  
      
</template>

<script>
export default {
  name: 'Project',
  props: {
  },
  data() {
        return {
            tempConvertUrl : "https://katy4599.github.io/Temp-Converter"
        }
  }
}
</script>

<style>

.project {
    text-align: center;
    font-family: Ubuntu, Helvetica, Arial, sans-serif;
}

.projectImg {
    width: 60% !important;
    height: 40% !important;
    padding-top: 15px;
    padding-bottom: 15px;
}

.desc {
    width: 60%;
    padding-left: 20%;
}
</style>