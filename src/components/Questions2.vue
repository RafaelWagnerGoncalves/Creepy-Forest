<template>
    <div class="container">
        <h2>Pergunta nº 2 - Ao ver que a manada passou, você desce da árvore e começa a explorar a região
        em busca de respostas. Não muito distante dali, você encontra um acampamento
        abandonado e um bilhete com instruções, deixado para trás. Antes que você possa
        alcançar o bilhete, um homem aparece com uma marreta gritando e avançando em
        sua direção. No seu corpo a adrenalina dispara. O que você faz?</h2>
    <div id="questions">
        <nuxt-link id="nuxtfail" to="/play/2/outcome/1"> a. Foge para bem longe</nuxt-link>
        <nuxt-link id="nuxtfail" to="/play/2/outcome/2"> b. Pega o bilhete e foge para bem longe</nuxt-link>
        <nuxt-link id="nuxtnext" to="/play/2/outcome/3"> c. Puxa toda coragem do coração e enfrenta o homem</nuxt-link>
    </div>
</div>   

</template>

<script>

export default {
    name: 'Questions2',
    props: {
        Quest2:String,
    }
};

</script>

<style scoped>
.container{
    height: 720px;
    background-image: url('../assets/camp.png');
    background-position: top center !important;
    background-repeat: repeat-x !important;
    background-color: #2c2b39 !important;
    background-size: cover !important;
    max-width: 1280px;
    margin-left:auto;
    margin-right:auto;
    box-sizing:border-box;
    max-height:720px;
    display:flex;
    flex-direction: column;
}

h2{
    color:rgb(255, 255, 255);
    padding:5px;
    text-align:justify;
    font-size:clamp(1rem, 2.5vw, 2rem); 
    margin:0;
    border-radius: 8px;
    outline: 1px solid rgba(0, 0, 0, 0.5);
    background-color: rgba(90, 90 , 90, 0.8)
}
#questions{
    box-sizing: border-box;
    margin-top:7vw;
    display:flex;
    justify-content:space-evenly ;

}
a{
    font-size: clamp(0.9rem, 2.0vw, 1.75rem);
    text-decoration: none;
    color: rgb(0, 0, 0);
    text-align: center;
    background-color: rgb(242 214 168 / 60%);
    max-width: 30%;
    border-radius: 8px;
    outline: 5px solid rgba(0, 0, 0, .5);
}
a:hover{
    color:orange;
}

@media (min-width: 598px) {
    a{
        padding:1rem;
    }
}
</style>
