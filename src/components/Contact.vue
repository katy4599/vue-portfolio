<template>
    <div class="contact">
      <h2>Feel free to contact me!</h2>
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
            linkedin: 'https://www.linkedin.com/in/'
        }
  }
}
</script>

<style>

.contact {
  text-align: center;
}

.icons {
  display: flex;
  flex-direction: row;
  align-items: center;
}

  .socialLink {
    width: auto;
    height: 75px;
    padding: 10px;
  }
</style>