<template>
    <header>
        <h1 id="titulo">{{ title }}</h1>
    </header>
</template>

<script>
export default {
    name: 'MainHeader',
    props: {
        title: String,
    }, 
}
</script>

<style scoped>
    header h1 {
        width:100%;
        background:black;
        background-size:cover;
        background-repeat: no-repeat;
        overflow:hidden;
        text-align:center;
        color:white;
    }

</style>
