<template>
    <div class="container">
        <h2 class="blood">Você Morreu!</h2>
        <p v-for="(text, id) in title" :key="id">{{ text }}</p>
        <nuxt-link id="nuxtstart" to="/">Jogar Novamente</nuxt-link>
    </div>
</template>

<script>
export default {
    name:'BadEnding',
    props: {
        title: Array,
    },
        
}
</script>

<style scoped>
.container{
    max-width:1280px;
    height:720px;
    background-image: url('../assets/pixeldead.jpg');
    background-repeat: repeat-x !important;
    background-size: cover !important;
    display:flex;
    flex-direction: column;
}
h2{
    height: 100px;
    color:rgb(139, 18, 18);
    list-style: none;
    margin-top:1em;
    text-align:center;
    font-size:clamp(1.3rem, 2vw + 1.2rem, 3rem);

}
h2:hover{color:rgba(53, 51, 51, 0.5);}
.blood{
    text-shadow:
       4px 4px 1px #300000,
       4px 6px 1px #400000,
       4px 8px 1px #500000,
       4px 10px 1px #600000,
       4px 12px 1px #700000,
       4px 14px 1px #800000,
       4px 16px 1px #900000,
       4px 18px 1px #A00000,
       4px 20px 1px #B00000,
       4px 22px 1px #C00000;
}
p{
    height: 100px;
    color:white;
    text-align:center;
    font-size:clamp(1rem, 2vw + 1rem, 2rem);
}
#nuxtstart {
    margin:auto;
    background-color: rgb(117, 30, 30);
    border: 0;
    border-radius: 56px;
    color: #fff;
    cursor: pointer;
    display: inline-block;
    font-family: system-ui,-apple-system,system-ui,"Segoe UI",Roboto,Ubuntu,"Helvetica Neue",sans-serif;
    font-size: 2vw;
    font-weight: 600;
    outline: 0;
    padding: 16px 21px;
    position: relative;
    text-align: center;
    text-decoration: none;
    transition: all .3s;
}
#nuxtstart:hover{
    color:rgb(255, 51, 0);
}


@media (min-width: 768px) {
  #nuxtstart {
    padding: 16px 48px;
  }
}

</style>