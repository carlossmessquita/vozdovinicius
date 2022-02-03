<template>

    <footer class="rodape">
        <p class="rodape-texto">Vinícius Sampaio - Locução e Narração Profissional  </p>
        <a :href="infoDev" class="rodape-link" target="_blank">Desenvolvido por Carlos Mesquita</a>
    </footer>
</template>

<script>
    export default {
        name: 'Footer',
        data() {
            return {
                infoDev: 'https://carlos-mesquita.herokuapp.com'
            }
        }
    }
</script>

<style scoped>
    .rodape {
        text-align: center;
        padding: 10px;
        background: #00ff95;
    }

    .rodape-link, .rodape-texto {
        margin: 1%;
        
        font-family: 'Rubik', sans-serif;
        font-size: 10px;
        text-decoration: none;
        font-style: italic;
        font-weight: bold;
        color: #080808;
    }

    .rodape-texto {
        font-style: normal;
        font-size: 12px;
        padding: 10px;
        border-bottom: 1px solid black;
    }
</style>