<template>
  <div id="app">
    <headtop />
    <router-view />
  </div>
</template>

<script>
import headtop from './components/HeadTop'
export default {
  components:{
    headtop
  }
}
</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  a {
    font-weight: bold;
    text-decoration: none;
    display: inline-block;
    width: 100%;
    height: 100%;
   
  }
}
</style>
