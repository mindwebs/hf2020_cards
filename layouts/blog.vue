<template>
  <div class="page">
    <Navbar />  
    <div class="body container">

      <a class="big-back-button" href="/">&lt;- Go back</a>

      <div v-if="page.image"> 
        <img :src="page.image" alt="page.title">
      </div>


      <h1 v-if="page.title">{{page.title}}'s page</h1>
      <slot name="default" />

      <div class="margined">
        <p class="card-text" v-if="page.socials">
          <strong>Socials: </strong>
          <span v-for="(social,index) in page.socials" :key="index">
            <a :href="social.url">{{social.name}}</a>&nbsp;
          </span>
          
        </p>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Navbar from '../components/Navbar.vue'
import Footer from '../components/Footer.vue'

export default {
  components: {
    Navbar,
    Footer
  },
  
  props: ['page']
}
</script>

<!-- This is global style -->
<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}

.container{
  width: 90%;
  max-width: 996px;
  margin: 0 auto;
}

.page{
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.page > * {
  flex-basis: 1;
}

.page .body{
  flex: auto;
  padding: 20px 0;
}

p{
    margin: 10px 0;
}

h1,h2,h3,h4,h5,h6{
    margin: 10px 0;
}


.margined{
  margin-top: 20px;
}

.big-back-button{
  font-size: 1.5rem;
}
</style>