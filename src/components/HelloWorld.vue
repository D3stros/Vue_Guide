<template>
  <div class="hello">
    <h1>{{title}}</h1>
    <Navbar />
  </div>
</template>

<script>
import Navbar from './Navbar'
export default {
  name: 'HelloWorld',
  components: {
    Navbar
  },
  data () {
    return {
      title: 'My first Vue app :)'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #444;
  font-weight: normal;
  text-align: center;
}
</style>
