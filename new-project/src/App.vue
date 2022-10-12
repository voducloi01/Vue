<template>
  <div id="app">
    <Vmodel />
  </div>
</template>

<script>

import Show from './Conditional/Show.vue';
import Vmodel from './Conditional/Vmodel.vue';
// import Search from './Search.vue'


export default {
    components: { Show, Vmodel } ,
   
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

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
 
}

a {
  color: #42b983;
}
</style>
