<template>
  <div class="container">
    <Header title="Jogo Desafio" />
  </div>
    <div class="wrapper">
      <Quest/>
    </div>
    <div class="wrapper2">
      <Quest2/>
    </div>
    <div class="wrapper3">
      <Quest3/>
    </div>
</template>

<script>
import Header from './components/Header'
import Quest from './components/Questions'
import Quest2 from './components/Questions2'
import Quest3 from './components/Questions3'

export default {
  name: 'App',
  components: {
    Header,
    Quest,
    Quest2,
    Quest3,
  },
}
</script>

<style>
html {
  margin:0;
  padding:0;
}
.wrapper{
  background-image: url("./assets/forestbackground.png");
  background-size:cover;
  box-sizing: border-box;
  background-repeat: no-repeat;
}
.wrapper2{
  background-image: url("./assets/camp.png");
  background-size:cover;
  box-sizing: border-box;
  background-repeat: no-repeat;
}
.wrapper3{
  background-image: url("./assets/abandoned_camp.jpg");
  background-size:cover;
  box-sizing: border-box;
  background-repeat: no-repeat;
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
