<template>
  <div id="backgroundstart">
    <nuxt-link id="nuxtstart" to="/play/1/">Start</nuxt-link>
  </div>
</template>

<script>
export default {
    name: 'Start',
    props: {
        title: String,
    }, 
}
</script>

<style scoped>
#backgroundstart {
  height:720px;
  max-width: 1280px;
  margin-left:auto;
  margin-right:auto;
  box-sizing:border-box;
  margin:auto;
  text-align:center;
  background-image:url("../assets/backgroundstart.png");
  background-size:cover;
  background-position:center;
  display:flex;
  align-items: center;
  justify-content:center;
}
#nuxtstart {
  background-color: rgb(26, 22, 22);
  border: 0;
  border-radius: 56px;
  color: #fff;
  cursor: pointer;
  display: inline-block;
  font-family: system-ui,-apple-system,system-ui,"Segoe UI",Roboto,Ubuntu,"Helvetica Neue",sans-serif;
  font-size: clamp(2rem, 2vw, 3rem);
  font-weight: 600;
  outline: 5px solid rgb(255, 255, 255);
  padding: 16px 21px;
  position: relative;
  text-decoration: none;
  transition: all .3s;
}

#nuxtstart:before {
  background-color: initial;
  background-image: linear-gradient(#fff 0, rgba(255, 255, 255, 0) 100%);
  border-radius: 125px;
  content: "";
  height: 50%;
  left: 4%;
  opacity: .5;
  position: absolute;
  top: 0;
  transition: all .3s;
  width: 92%;
}

#nuxtstart:hover {
  box-shadow: rgba(255, 255, 255, .2) 0 3px 15px inset, rgba(0, 0, 0, .1) 0 3px 5px, rgba(0, 0, 0, .1) 0 10px 13px;
  transform: scale(1.05);
}

@media (min-width: 768px) {
  #nuxtstart {
    padding: 16px 48px;
  }
}
    
</style>
