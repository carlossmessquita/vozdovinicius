<template>  

        <main class="principal">
            <div class="container-principal">
                <div class="imagens-titulo">
                    <img src="media/fotositectd.png" alt="Foto de Perfil" class="perfil">
                    <img src="media/logosite1ctd.png" alt="Logo do Site" class="logo">
                </div>

                <div class="imagens">
                    <img src="media/rostopng.png" alt="Logo de rosto falando" width="60px" height="60px">
                    <h2 class="subtitulo">Conecto empresas e clientes através de uma interpretação de qualidade.</h2>
                </div>

                <div class="imagens">
                    <img src="media/foguete.png" alt="Logo de Foguete" width="55px" height="55px" class="foguete">
                    <h2 class="subtitulo2">Foco no seu briefing sem esquecer da qualidade de áudio e do prazo de
                        entrega.</h2>
                </div>

                <a class="link" :href="whatsapp" target="_blank">SOLICITE UM ORÇAMENTO!</a>
            </div>
        </main>
</template>

<script>
    export default {
        name: 'Informacoes',
        data() {
            return {
                whatsapp: 'https://api.whatsapp.com/send?phone=5585999069198'
            }
        }
    }
</script>

<style scoped>
    .container {
        display: flex;
        align-items: center;
        justify-content: space-evenly;
    }

    .container-principal {
        display: flex;
        flex-direction: column;
        width: auto;
    }


    .imagens, .imagens-titulo {
        display: flex;
        align-items: center;
        justify-content: space-evenly;
        font-size: 16px;
    }

    .foguete {
        margin-left: 2%;
    }

    .logo{
        width: 380px;
        height: 200px;
        margin: 5%;
    }

    .perfil {
        width: 200px;
        height: 200px;
        margin: 2%;
    }


    .link {
        border: 3px solid #00ff95;
        border-radius: 20px;
        margin: 5%;
        padding: 8px;
        font-size: 15px;
        text-decoration: none;
        text-align: center;
        color: #00ff95;
        font-family: 'Montserrat', sans-serif;
        font-weight: bold;
    }

    .link:hover {
        color: #080808;
        background: #00ff95;
    }

@media (max-width: 940px) {

        .container-principal {
            padding: 5%;
            margin: 0;
        }

        .link {
            margin: 10% auto;
        }

        .imagens-titulo {
            display: flex;
            flex-direction: column;
        }

        .logo {
            width: 300px;
            height: 200px;
        }
        
        .perfil {
            width: 200px;
            height: 200px;
        }

        .foguete {
            margin-left: 0%;
        }

        .subtitulo2 {
            margin-left: 2%;
            margin-top: 4%;
        }

        .subtitulo-rep {
            text-align: center;
        }
    }
</style>