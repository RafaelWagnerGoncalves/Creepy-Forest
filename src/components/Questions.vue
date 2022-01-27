<template>
    <div class="container">
        <div id="divh2">
        <h2>Pergunta nº 1 - Você acordou na floresta tonto e com uma grande dor de cabeça, sem nenhuma
        memória de como foi parar ali. Um barulho cada vez mais intenso foi o que
        despertou você desse apagão. Após abrir os olhos e levantar-se, você observa uma
        manada de búfalos vindo em sua direção, a pouquíssimos metros de distância. O
        que você faz?</h2>
        </div>
    <div id="questions">
        <nuxt-link id="nuxtfail" to="/play/1/outcome/1"> a. Corre o mais rápido possível</nuxt-link>
        <nuxt-link id="nuxtnext" to="/play/1/outcome/2"> b. Sobe na árvore</nuxt-link>
        <nuxt-link id="nuxtfail" to="/play/1/outcome/3"> c. Se finge de morto</nuxt-link>
    </div>
    </div>
</template>

<script>

export default {

    name: 'Questions',
    props: {
        Quest:String,
    }
};
</script>

<style scoped>

.container{
    height: 720px;
    background-image: url('../assets/forestbackground.png');
    background-position: top center !important;
    background-repeat: repeat-x !important;
    background-color: #2c2b39 !important;
    background-size: cover !important;
    color:white;
    max-width: 1280px;
    margin-left:auto;
    margin-right:auto;
    box-sizing:border-box;
    max-height:720px;
    display:flex;
    flex-direction: column;
    
    
}
#divh2{
 max-height: 720px;
}

h2{
    color:White;
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
