<template>
     <div id="sobre" style="position: absolute;top: 160%;"></div>
    <section class="container-fluid section__container--two">
        <div class="section__container__informations--app">
            <h3>
                O que é o <strong>Vistoria Solar ?</strong>
            </h3>
           <p>
            O aplicativo de vistoria solar é uma solução intuitiva e fácil de usar para otimizar o processo de inspeção de imóveis. Ele inclui um módulo web para gerenciamento e acompanhamento das vistorias. Com uma abordagem agradável e organizada, o aplicativo recebe aprovação total dos especialistas, sendo essencial para o sucesso das vistorias.   
            <br>
            <br>
            <button class="btn text-bg-info button__app" style="background-color: var(--color-green-2) !important;">Fazer cadastro</button>
           </p>
        </div>
        <div>
            <section class="container section__container--img">
               <img src="../../../assets/painel-solar.png"  alt="Logo Vistoria Solar" class="img-fluid">
            </section>
        </div>
    </section>

    <section>
        <Slide />
    </section>
</template>

<script>
    import './styles/style.css'
    import Slide from '../section_slide/section_slide.vue'

    export default {
        components: {
            Slide
        }
    }
</script>

<style scoped>
.section__container--two {
    background: var(--color-green-1);
    
}

.section__container--two h3 { 
    font-size: var(--gap-32);
    font-weight: 800;
    color: var(--color-white-1);
}

.section__container--two p {
    font-size: 17px;
    color: var(--color-white-1);
    text-align: left;
}
.section__container__informations--app {
    margin-right: var(--gap-128);
}

.section__container__informations--app h3 {
    text-align: left;
    margin-bottom: var(--gap-32);
}
.section__container--img {
    max-width: 400px;
}

@media screen and (max-width: 990px) {
    .button__app {
       margin: 0 auto !important;
    }
}
</style>

