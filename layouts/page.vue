<template>
  <div class="page">
    <Navbar />  
    <div class="body container">
      <slot name="default" />
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
  }
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
  max-width: 1024px;
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

</style>