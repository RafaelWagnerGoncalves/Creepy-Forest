<template>
    <div class="container">
        <h2>Pergunta nº 3 - Você finalmente consegue ler o bilhete: “Vamos fazer parecer um acidente. Misture o
        conteúdo deste frasco na comida dele. O remédio vai começar a fazer efeito depois
        de 30 minutos. Quando ele estiver completamente apagado, leve-o até o pé da
        árvore mais alta no início da floresta e direcione a manada de búfalos em sua
        direção. Estaremos esperando no laboratório ao norte do acampamento.” O que
        você faz?</h2>
    <div id="questions">
        <nuxt-link id="nuxtnext" to="/play/3/outcome/1"> a. Foge e liga para a polícia</nuxt-link>
        <nuxt-link id="nuxtfail" to="/play/3/outcome/2"> b. Amarra o homem e vai ao laboratório</nuxt-link>
        <nuxt-link id="nuxtfail" to="/play/3/outcome/3"> c. Mata o homem, pega a marreta e vai ao laboratório</nuxt-link>
    </div>    
        </div>
</template>

<script>

export default {
    name: 'Questions3',
    props: {
        Quest3:String,
    }
};

</script>

<style scoped>
.container{
    height: 720px;
    background-image: url('../assets/abandoned_camp.jpg');
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
    margin-top:15vw;
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