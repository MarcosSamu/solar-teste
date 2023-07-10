<template class="mb-auto" >
    <div id="servicos" style="position: absolute;top: 80%;"></div>
    <section class="container-fluid container__section--one" >
        <div class="text-center row " style="justify-content: center;">
            <div class="col-4 section__one--spacing">
                <h3 class="title">Nossos principais recursos</h3>
                <p class="subtitle">
                    Conheça as funcionalidades do Solar Vistorias e otimize o tempo usando o melhor do mercado
                </p>
            </div>
        </div>

        <div class="section__one--informations">
            <div class="card card-flex-position" style="width: 40rem;">
                <img src="../../../assets/icons/agility.png" class="icon_img card-img-top" alt="Agilidade da aplicação">
                <div class="card-body">
                    <h5 class="card-title">Agilidade</h5>
                    <p class="card-text">
                        Aumenta a eficiência ao simplificar as inspeções, diminuindo o tempo necessário para o vistoriador e a imobiliária
                    </p>
                </div>
            </div>
            <div class="card card-flex-position" style="width: 40rem;">
                <img src="../../../assets/icons/wifi.png" class="icon_img card-img-top" alt="Sem Wifi">
                <div class="card-body">
                    <h5 class="card-title">Visita Offline</h5>
                    <p class="card-text">Não é preciso estar conectado à internet para realizar a inspeção no local do imóvel.</p>
                </div>
            </div>
            <div class="card card-flex-position" style="width: 40rem;">
                <img src="../../../assets/icons/oclock.png" class="icon_img card-img-top" alt="Armazenamento">
                <div class="card-body">
                    <h5 class="card-title">Relatórios Dinâmicos</h5>
                    <p class="card-text">
                        Exploraremos como criar e utilizar relatórios personalizados que se ajustam dinamicamente às demandas da sua empresa.
                    </p>
                </div>
            </div>
            <div class="card card-flex-position" style="width: 40rem;">
                <img src="../../../assets/icons/photo.png" class="icon_img card-img-top" alt="Foto">
                <div class="card-body">
                    <h5 class="card-title">Multimidia</h5>
                    <p class="card-text">forneceremos informações e orientações essenciais, juntamente com fotos e vídeos, para realizar uma vistoria completa e precisa.</p>
                </div>
            </div>
            <div class="card card-flex-position" style="width: 40rem;">
                <img src="../../../assets/icons/default.png" class="icon_img card-img-top" alt="Padrão">
                <div class="card-body">
                    <h5 class="card-title">Padronização</h5>
                    <p class="card-text">Promove a padronização de relatórios, onde o sistema gera automaticamente os laudos após a conclusão de cada inspeção.</p>
                </div>
            </div>
            <div class="card card-flex-position" style="width: 40rem;">
                <img src="../../../assets/icons/cursor.png" class="icon_img card-img-top" alt="Ponteiro">
                <div class="card-body">
                    <h5 class="card-title">Sem digitação</h5>
                    <p class="card-text">Elimina a necessidade de digitar manualmente os relatórios, reduzindo assim os erros ortográficos</p>
                </div>
            </div>
        </div>
    </section>

    <SectionTwo />
</template>

<script>
import './styles/style.css'
import SectionTwo from '../section_two/section_two.vue'

export default {
    components: {
        SectionTwo  
    }
}
</script>

<style scoped>
    .section__one--informations .card {
        background-color: transparent;
        border: 0;
        margin: 0 auto;
    }
    .section__one--informations .card .card-body {
        text-align: center;
    }

    img.icon_img  {
        width: var(--gap-64);
        height: var(--gap-64);
        margin: 0 auto;
    }
    .card-flex-position {
        display: flex !important;
        flex-direction: row;
        align-items: center;
        justify-content: space-around;
    }
</style>


