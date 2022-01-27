<template>
    <div class="container">
        <p>a. Foge e liga para a polícia<br>Você informa a polícia o que aconteceu e passa a localização do
laboratório.<br>Chegando lá ela se depara com um sítio de produção de cocaína
e prende todos os presentes.<br> As evidências sugerem que você ainda pode
estar em perigo, por este motivo a polícia lhe coloca no programa de
proteção à testemunha e você sobrevive para vivenciar uma nova história.<br>
Parabéns, você ganhou!
</p>
    <div id="questions">
        <nuxt-link id="nuxtnext" to="/">Terminar</nuxt-link>
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
    background-image: url('../assets/celebrating.gif');
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
    background-color: rgba(17, 216, 33, 0.4)
}

#nuxtnext {
    max-width: 4rem;
    max-height: 2rem;
    background-color: rgb(255, 255, 255);
    border: 0;
    border-radius: 10px;
    color: rgb(0, 0, 0);
    cursor: pointer;
    font-family: system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, Noto Sans, sans-serif,system-ui,"Segoe UI",Roboto,Ubuntu,"Helvetica Neue",sans-serif;
    font-size: clamp(1.1rem, 2vw, 3rem);
    font-weight: 600;
    outline: 5px solid rgba(0, 0, 0, 0.8);
    padding: 0.5rem 1.7rem;
    text-decoration: none;
    transition: all .3s;
    margin: 0 auto;
    text-align: center;
    display: flex;
    align-items: center;
    justify-items: center;
}

@media (min-width: 768px) {
  #nuxtnext {
    width:20%;
    font-size:1.1rem;
  }
}


</style>
