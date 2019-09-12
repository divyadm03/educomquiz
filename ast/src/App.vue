<template>
  <div id="app">
    <div id="nav">
      <Quiz></Quiz>
    </div>
    <router-view/>
  </div>
</template>


<script>
 import Quiz from './components/Quiz.vue'
export default {
  name: 'app',
  components :{
    Quiz
  }
}
</script>
<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
