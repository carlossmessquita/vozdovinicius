<template>
    <Navbar />
    <div class="container">
        <Informacoes />
        <Conteudo />  
    </div>
    
    <Footer />
</template>

<script>
    import Navbar from './components/Navbar.vue';
    import Informacoes from './components/Informacoes.vue';
    import Conteudo from './components/Conteudo.vue';
    import Footer from './components/Footer.vue';

    export default {
        name: 'App',
        components: {
            Navbar,
            Informacoes,
            Conteudo,
            Footer
        }
    }
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Rubik:wght@300&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Titillium+Web:wght@200&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300&display=swap');

    /* Código CSS*/
    body {
        background-image: linear-gradient(to left top, #000000, #080808, #0e0e0e, #141414, #181818, #19191a, #1b1b1b, #1c1c1d, #1b1b1d, #191b1c, #171a1b, #161a1a);
        background-position: center;
        color: #00ff95;
    }

    /* Works on Firefox */
    * {
    scrollbar-width: 0px;
    }
    
    /* Works on Chrome, Edge, and Safari */
    *::-webkit-scrollbar {
    width: 0px;
    }

    .container {
        display: flex;
        align-items: center;
        margin: auto auto 6%;
        justify-content: space-around;
        
    }

    .subtitulo, .subtitulo2, .subtitulo-rep {
        padding: 5px;
        font-size: 20px;
        font-family: 'Rubik', sans-serif;
        font-weight: bold;
        
    }

    .subtitulo-rep {
        margin: 2%;
    }

    .subtitulo2 {
        margin-left: 4%;
    }

    .titulo {
        padding: 10px;
        font-size: 25px;
        text-align: center;
        color: #00ff95;
        font-family: 'Rubik', sans-serif;
        font-weight: bold;
        margin-bottom: 5px;
    }

    /* Responsividade */

    @media (max-width: 940px) {
        .container {
            display: flex;
            flex-direction: column;
        }


    }
</style>
