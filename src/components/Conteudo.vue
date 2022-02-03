<template> 
    
        <section class="portfolio">
            <div class="container-portfolio">
                <h1 class="titulo" >REPERTÓRIO</h1>
                <div class="audioplayer" v-for="audio in arquivos" :key="audio.id"> 
                    <h1 class="subtitulo-rep"> {{ audio.titulo}} </h1>
                    <audio controls="controls">
                        <source  :src="audio.src" type="audio/mpeg" />
                        Your browser does not support the audio element.
                    </audio> 
                </div>


            </div>
    </section>
</template>

<script>
    export default {
        name: 'Conteudo',
        data() {
            return {
                arquivos: [
                    {id:1, titulo:'Narração', src:'audios/ViniciusSampaioNarracao.mp3'},
                    {id:2, titulo:'Repertório Nordestino', src:'audios/ViniciusSampaioNordestino.mp3'},
                    {id:3, titulo:'Voz Jovem', src:'audios/ViniciusSampaioJovem.mp3'}
                ]
            }
        }
    }
</script>

<style scoped>
    .container-portfolio {
        display: flex;
        flex-direction: column;
        padding: auto;
        margin: auto auto 6%;

    }

    .controls {
        background: #080808;
    }

    @media (max-width: 940px) {
        .container-portfolio {
            margin-bottom: 10%;
        }
        .subtitulo-rep {
            text-align: center;
        }
    }
</style>