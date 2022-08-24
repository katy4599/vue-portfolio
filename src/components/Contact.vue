<template>
    <div class="contact">
      <h1 class="title">Feel free to contact me!</h1>
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
      <form name="contact" method="POST" content-type="application/x-www-form-urlencoded" data-netlify="true" netlify>
        <p>
          <label>Your Name: <input type="text" name="name" /></label>
        </p>
        <p>
          <label>Your Email: <input type="email" name="email" /></label>
        </p>
        <p>
          <label>Your Role: <select name="role[]" multiple>
            <option value="leader">Leader</option>
            <option value="follower">Follower</option>
          </select></label>
        </p>
        <p>
          <label>Message: <textarea name="message"></textarea></label>
        </p>
        <p>
          <button type="submit">Send</button>
        </p>
      </form>

      
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

<style scoped>

.contact {
  text-align: center;
  margin-top: 2.5%;
  font-family: Ubuntu, Helvetica, Arial, sans-serif;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.title {
  width: 100%;
}
.icons {
  
  width: 100%;
}


  .socialLink {
    width: 4rem;
    height: 4rem;
    padding: 15px;
  }

  
</style>