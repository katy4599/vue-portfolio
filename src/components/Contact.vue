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
      <div>
        <form netlify @submit.prevent="handleSubmit" name="contact" method="POST" netlify-honeypot="bot-field" data-netlify="true">
          <p style="display: none;" class="hidden">
            <label>Don't fill this out if you are human: <input name="bot-field" /></label>
          </p>
          <p>
            <label>Your Name: <input v-model="form.name" type="text" name="name" /></label>
          </p>
          <p>
            <label>Your Email: <input v-model="form.email" type="email" name="email" /></label>
          </p>
          <p>
            <label>Message: <textarea v-model="form.message" name="message"></textarea></label>
          </p>
          <p>
            <button type="submit">Send</button>
          </p>
        </form>
      </div>
    </div>  
      
</template>

<script>
export default {
  name: 'Contact',
  
  data () {
    return {
      form: {
        name: '',
        email: '',
        message: ''
      },
      github: 'https://github.com/katy4599',
      linkedin: 'https://www.linkedin.com/in/katy-millard'
    }
  },
  
  methods: {
    encode(data) {
      return Object.keys(data)
      .map(key => `${encodeURIComponent(key)}=${encodeURIComponent(data[key])}`)
      .join('&')
    },
    handleSubmit() {
      fetch('/', {
        method: 'post',
        headers: {
          "Content-Type": "application/x-www-form-urlencoded"
        },
        body: this.encode({
          'form-name': 'contact',
          ...form
        })
      })
      .then(() => console.log('successfully sent'))
      .catch(e => console.error(e))
    }
  }
}
</script>

<style>

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