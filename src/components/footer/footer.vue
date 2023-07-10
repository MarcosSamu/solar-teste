<template>
    <MapSvg />    
    <div id="contato"></div>

    <div class="container-fluid footer__container">
    <footer class="container d-flex container__footer__content flex-wrap mb-1 justify-content-between align-items-center py-3 my-4 ">
        <div class="col-md-4 d-flex align-items-center">
        <a href="/" class="mb-3 me-2 mb-md-0 text-muted text-decoration-none lh-1">
            <img src="../../assets/Logo.png" alt="Logo da vistoria solar" class="img-fluid">
        </a>
        <span class="mb-3 mb-md-0  text__title__footer">&copy; 2023 Vistoria Solar</span>
        </div>

   
        <ul class="nav col-md-4 justify-content-center list-unstyled d-flex" id="links">
            <li class="ms-3"><a href="https://wa.me/5586999405102" class="text-muted" ><svg class="bi" width="24" height="24"><use xlink:href="#twitter"/></svg></a></li>
            <li class="ms-3"><a class="text-muted" href="https://www.instagram.com/exataengenhariapi"><svg class="bi" width="24" height="24"><use xlink:href="#instagram"/></svg></a></li>
            <li class="ms-3"><a class="text-muted" href="#"><svg class="bi" width="24" height="24"><use xlink:href="#facebook"/></svg></a></li>
        </ul>
    </footer>
    </div>
</template>

<script>
import MapSvg from './svgMap.vue'

export default {
    components: {
        MapSvg
    }
}
</script>

<style scoped>
    .footer__container {
        position: relative;
        margin-top: var(--gap-32);
        background: var(--color-green-1);
        padding:calc(var(--gap-32) + 3px);
    }

    .nav .ms-3 a {
        fill: var(--color-green-2);
    }

    span.text__title__footer{
        color: var(--color-green-2);
    }

    .d-flex {
        display: flex !important;
        flex-wrap: wrap;
        justify-content: center;
    }


    @media screen and (max-width: 990px) {
        .footer__container[data-v-676f3426] {
            position: relative;
            margin-top: 32vh;
            background: var(--color-green-1);
            padding: calc(var(--gap-32) + 1px);
        }

        #links {
            margin: 0 auto;
        }
    }
</style>