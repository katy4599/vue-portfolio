<template>
    <div class="exp">
      <h1>Experience</h1>
      <div class="work">
  
        <img src="@/assets/SnapIT.webp" />
        <h3>SnapIT Solutions<br>
          Overland Park, Kansas<br>
          Junior Software Developer</h3>
        <p>After successfully completing a fundamental JavaScript training,
          I began a four month apprenticeship. During this time I added several 
          JS frameworks to my skills. In August 2022, I was welcomed to the SnapIT Solutions
          team as a full time Junior Software Developer.
        </p>
      </div>
      <div>
        <h1>Skills</h1>
        <ul class="list">
          <li>JavaScript</li>
          <li>HTML/CSS</li>
          <li>GitHub</li>
          <li>React</li>
          <li>Vue</li>
          <li>Node</li>
        </ul>
      </div>
    </div>
</template>

<script>
export default {
  name: 'Experience',
  props: {
  }
}
</script>

<style>

.exp {
  text-align: center;
  font-family: Ubuntu, Helvetica, Arial, sans-serif;
}

.work h3 {
  font-size: .8rem;
  margin-top: -12%;
  margin-left: 34%;
  text-align: left;
  margin-right: 10% !important;
  
}

.work p {
  width: 80% !important;
  margin-top: 25px;
}

.work {
  width: 100%;
  margin-left: 10%;
  margin-right: 10%;
}

.exp img {
  width: 75px !important;
  height: 75px !important;
  margin-right: 375px;
  margin-left: 15%;
}

.list {
  text-align: left;
  margin-left: 35%;
}
</style>