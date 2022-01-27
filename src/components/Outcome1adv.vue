<template>
    <div class="container">
            <p>Escolha: Sobe na árvore<br>  >Você sobe na árvore e escapa por pouco da manada</p>
        
            <nuxt-link id="nuxtnext" to="/play/2"> Avançar </nuxt-link>
    
    </div>
</template>

<script>

export default {

    name: 'Outcome1adv',
    props: {
        Quest:String,
    }
};
</script>

<style scoped>
*{
    color:white;
}
.container{
    background-image: url('../assets/forestbackground.png');
    background-position: top center !important;
    background-repeat: repeat-x !important;
    background-color: #2c2b39 !important;
    background-size: cover !important;
    height: 720px;
    max-width:1280px;
    display:flex;
    flex-direction: column;
    align-items:center;

}

p{
    padding:5px;
    text-align:center;
    font-size:clamp(1.3rem, 2.5vw, 2rem); 
    margin-bottom:10vw;
    border-radius: 8px;
    outline: 1px solid rgba(0, 0, 0, 0.5);
    background-color: rgba(90, 90 , 90, 0.8)
}


#nuxtnext {
    background-color: rgb(9, 184, 24);
    border: 0;
    border-radius: 56px;
    color: #fff;
    cursor: pointer;
    font-family: system-ui,-apple-system,system-ui,"Segoe UI",Roboto,Ubuntu,"Helvetica Neue",sans-serif;
    font-size: clamp(1.1rem, 2vw, 3rem);
    font-weight: 600;
    outline: 5px solid rgba(0, 0, 0, 0.8);
    padding: 16px 21px;
    text-decoration: none;
    transition: all .3s;
    width:16%;
    margin:0 auto;
    text-align:center;
}
#nuxtnext:hover{
    color:black;
}


</style>
