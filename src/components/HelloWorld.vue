<template>
  <div class="hello">
    <h1>{{title}}</h1>
    <Navbar />
    <AllFriends :friends="friends" />
    <OnlineFriends :friends="friends" />
  </div>
</template>

<script>
import Navbar from './Navbar'
import AllFriends from './AllFriends'
import OnlineFriends from './OnlineFriends'

export default {
  name: 'HelloWorld',
  components: {
    Navbar,
    OnlineFriends,
    AllFriends
  },
  data () {
    return {
      title: 'My first Vue app :)',
      friends: [
        { name: 'Mario', online: true },
        { name: 'Luigi', online: false },
        { name: 'Toad', online: true },
        { name: 'Bowser', online: false }
      ]
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
