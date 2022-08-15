<template>
    <div class="contact">
      <h1>Feel free to contact me!</h1>
      <div class="icons">
        <a :href="linkedin">
          <img class="socialLink" src="@/assets/LinkedIn.webp" />
        </a>  
        <a :href="github">
          <img class="socialLink" src="@/assets/GitHub.webp" />
        </a>
        <a href="mailto: katy.millard@gmail.com">
          <img class="socialLink" src="@/assets/Email.png" />
        </a>
      </div>
      
    </div>  
      
</template>

<script>
export default {
  name: 'Contact',
  props: {
  },
  data() {
        return {
            github: 'https://github.com/katy4599',
            linkedin: 'https://www.linkedin.com/in/katy-millard'
        }
  }
}
</script>

<style>

.contact {
  text-align: center;
  margin-top: 30%;
  font-family: Ubuntu, Helvetica, Arial, sans-serif;
}

.icons {
  display: flex;
  flex-direction: row;
  align-items: center;
  margin-bottom: 50px;
}

  .socialLink {
    width: 4rem;
    height: 3rem;
    padding: 0px;
  }

  
</style>