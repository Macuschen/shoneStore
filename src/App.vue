<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <router-view/>
    <div>{{a}}</div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data(){
    return {
      a:10
    }
  },
  created () {
    console.log(this.$store.state)
  },
  mounted() {
    console.log(this.$store.state);
    
  },
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
