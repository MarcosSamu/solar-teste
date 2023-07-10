<template>
    <section class="parallax-section">
        <div class="container banner__hero">
            <h1>
               <strong>Solar Vistorias</strong>
                <br>
                Simples, rápido e eficiente
            </h1>
            <a class="btn text-bg-info" target="_blank" href="https://alfaweb.meugestorsolar.com/"  style="background-color: var(--color-green-2) !important;">Fazer cadastro</a>
        </div>
    </section>
</template>
<script>
  import './styles/styles.css'
</script>

<style scoped>
    .parallax-section {
        width: 100%;
        height: 90vh;
        display: flex;
        align-items: center;
        justify-content: center;

        text-align: center;
    }
    .parallax-section {
        position: relative;
    }
    .parallax-section::before {
        content: '';
        position: absolute;
        left: 0;
        top: 0;
        background: radial-gradient(rgba(29, 39, 17, 0.5), transparent);
        width: 100%;
        height: 100%;
        z-index: 0;
    }
    .banner__hero {
        z-index: 1;
    }
    .banner__hero h1 {
        font-size: 4rem;
        color: var(--color-white-1);
        z-index: 10000000;
       
    }
    .banner__hero h1 strong {
        font-weight: 900;
    }


    @media screen and (max-width: 990px) {
        .banner__hero h1 {
            font-size: 2.5rem;
        }
    }
</style>