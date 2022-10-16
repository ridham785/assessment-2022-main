<template>
  <div id="app">
    <div style="position: absolute; bottom: 0px; right: 0px;">
      <img v-bind:src="img"/>
    </div>
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/challenge-1">Challenge 1</router-link> | 
      <router-link to="/challenge-2">Challenge 2</router-link> | 
      <router-link to="/challenge-3">Challenge 3</router-link> |
      <router-link to="/final">Final</router-link>
    </div>
    <router-view/>
  </div>
</template>

<script>
    export default {
        
        data() {
            return {
                img: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSUFoRSJIqxKVGkvje2lFQZnyGT-SjeOXmh-0Yl9PWWFQ&s'
            }
        }
    }
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
