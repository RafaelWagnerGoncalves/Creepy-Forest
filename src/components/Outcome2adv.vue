<template>
    <div class="container">
        <p>Puxa toda coragem do coração e enfrenta o homem<br>
> Você consegue desviar da primeira marretada do homem, que fica ocioso
por um curto período, o suficiente para você acertá-lo em cheio na cabeça e
apagá-lo no chão.
</p>
    <div id="questions">
        <nuxt-link id="nuxtnext" to="/play/3"> Avançar</nuxt-link>
    </div>
</div>   

</template>

<script>

export default {
    name: 'Outcome2adv',
    props: {
        Quest2:String,
    }
};

</script>

<style scoped>
.container{
    background-image: url('../assets/camp.png');
    background-position: top center !important;
    background-repeat: repeat-x !important;
    background-color: #2c2b39 !important;
    background-size: cover !important;
    height: 720px;
}
#questions{
    box-sizing:border-box;
    padding:5vw;
    height:287px;
    width:100%;
    display:flex;
}
p{
    Color:white;
    padding:5px;
    text-align:center;
    font-size:clamp(1.3rem, 2.5vw, 2rem); 
    margin:0;
    border-radius: 8px;
    outline: 1px solid rgba(0, 0, 0, 0.5);
    background-color: rgba(90, 90 , 90, 0.8)
}
#nuxtnext {
    margin:auto;
    background-color: rgb(9, 184, 24);
    border: 0;
    border-radius: 56px;
    color: #fff;
    cursor: pointer;
    display: flex;
    font-family: system-ui,-apple-system,system-ui,"Segoe UI",Roboto,Ubuntu,"Helvetica Neue",sans-serif;
    font-size: clamp(1.1rem, 2vw, 3rem);
    font-weight: 600;
    outline: 5px solid rgba(0, 0, 0, 0.8);
    padding: 16px 21px;
    position: relative;
    text-align: center;
    text-decoration: none;
    transition: all .3s;
}
#nuxtnext:hover{
    color:black;
}


@media (min-width: 768px) {
  #nuxtnext {
    padding: 16px 48px;
  }
}

</style>
