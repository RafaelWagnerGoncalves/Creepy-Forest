<template>
  <div class="container">
    <div id="startgame"><Start />
    </div>
  </div>
</template>

<script>
import MainHeader from '../src/components/MainHeader.vue'
import Start from '../src/components/Start.vue'


export default {
  name: 'App',
  components: {
    MainHeader,
    Start,
  },
}
</script>

<style>

#startgame{
  width:100%;
}

body {
  margin:0;
  padding:0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #1b1a1a;
}
</style>
