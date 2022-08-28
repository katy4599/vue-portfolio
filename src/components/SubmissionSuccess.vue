<template>
  <div class="msg">
    <h1>It does work! Thank you for your submission!</h1>
    <router-link to="/">
      <button>Back to Home</button>
    </router-link>
  </div>
</template>

<script>
  export default {
    name: "SubmissionSuccess"
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
.msg {
    margin-top: 10%;
}

</style>