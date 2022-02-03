<template>
    
    <div class="cabecalho">
        <div class="container-cabecalho">
            
            <div class="contato">
                <img src="media/instagram.png" alt="Instagram" class="insta">
                <a :href="insta" class="link-contato" target="_blank">Instagram</a>
            </div>

            <div class="contato">
                <img src="media/wpp.png" alt="Instagram" class="insta">
                <a :href="whatsapp" class="link-contato" target="_blank">Whatsapp</a>
            </div>

            <div class="contato">
                <img src="media/email.png" alt="Email">
                <a :href="email" class="link-contato" target="_blank">Email</a>
            </div>

        </div>
    </div>
</template>

<script>

    export default {
        name: 'Navbar',
        data() {
            return {
                insta: 'https://www.instagram.com/vozdovinicius/',
                email: 'mailto:vozdovinicius@gmail.com',
                whatsapp: 'https://api.whatsapp.com/send?phone=5585999069198'
            }

        }
    }
</script>

<style scoped>
    .contato {
        display: flex;
        align-items: center;
    }

    .insta {
        width: 20px;
        height: 20px;
    }

    .container-cabecalho {
        display: flex;
        justify-content: space-evenly;
        padding: 10px;
        background: #00ff95;
        align-items: center;
    }

    .link-contato {
        padding: 5px;
        text-decoration: none;
        font-family: 'Montserrat', sans-serif;
        font-weight: bold;
        font-size: 15px;
        color: #080808;
    }
</style>