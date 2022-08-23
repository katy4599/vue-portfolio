<template>
    <div class="project2">
      <h1>Featured Projects (cont'd)!</h1>
      <div class="rps">
        <h3>Rock-Paper-Scissors</h3>
        <img class="projectImg" src="@/assets/RPS.png" />
        <p class="desc">As an apprentice assignment, this JavaScript project uses 
            session storage to maintain the score to the classic Rock-Paper-Scissors
            game. The score only resets when the New Game button is clicked.</p>
        <a :href="rpsUrl">
            <p>Try it Live!!!</p>
        </a>  
      </div>
    </div>  
      
</template>

<script>
export default {
  name: 'Project2',
  props: {
  },
  data() {
        return {
            rpsUrl : "https://katy4599.github.io/rock-paper-scissors"
        }
  }
}
</script>

<style scoped>

.project2 {
    text-align: center;
    font-family: Ubuntu, Helvetica, Arial, sans-serif;
    margin-top: 10px;
    margin-bottom: 10px !important;
}

.projectImg {
    width: 60% !important;
    height: 40% !important;
    /* padding-top: 10px; */
    /* padding-bottom: 15px; */
}

.desc {
    width: 60%;
    padding-left: 20%;
    margin-bottom: 10px;
}
</style>