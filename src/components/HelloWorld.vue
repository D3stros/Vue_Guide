<template>
  <div class="hello">
    <h1>{{title}}</h1>
    <Navbar />
    <Blogs />
  </div>
</template>

<script>
import Navbar from './Navbar'
import Blogs from './Blogs'

export default {
  name: 'HelloWorld',
  components: {
    Navbar,
    Blogs
  },
  data () {
    return {
      title: 'My first Vue app :)'
    }
  },
  methods: {

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
