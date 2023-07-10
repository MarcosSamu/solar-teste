<template id="container__three">
<div id="baixe" style="position: absolute;top: 230%;"></div>
<h1 class="title text-center title-slide">Entenda mais sobre nosso app</h1>
   <div class="container container__slide">
       <div class="img-fluid">
            <img src="../../../assets/frame.png" alt="">
       </div>
       <div class="cards slide__card mt-5">
           <div class="card">
                <h2>
                    Controle pelo celular
                </h2>
                <p>
                    Oferece uma experiência de usuário excepcional, aderindo aos princípios de engenharia de usabilidade.
                </p>
           </div>
       </div>

       <div class="cards slide__card">
           <div class="card">
                <h2>
                    Multiplataforma
                </h2>
                <p>
                    Utilize seu dispositivo móvel ou computador para desfrutar dos nossos serviços de maneira conveniente e acessível.
                </p>
           </div>
       </div>

       <div class="cards slide__card">
        
           <div class="card">
                <h2>
                    Informação
                </h2>
                <p>
                    Agilidade na busca de informações e fotos da vistoria, quando necessário, todo histórico é disponível no sistema.
                </p>
                
            </div>
        </div>
        
    </div>
    <center>
        <button  data-bs-toggle="modal" data-bs-target="#exampleModal" id="qrcode__icon" > Baixe aqui nosso app 
            <span style="margin-left: 8px;"></span>
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-qr-code-scan" viewBox="0 0 16 16">
                <path d="M0 .5A.5.5 0 0 1 .5 0h3a.5.5 0 0 1 0 1H1v2.5a.5.5 0 0 1-1 0v-3Zm12 0a.5.5 0 0 1 .5-.5h3a.5.5 0 0 1 .5.5v3a.5.5 0 0 1-1 0V1h-2.5a.5.5 0 0 1-.5-.5ZM.5 12a.5.5 0 0 1 .5.5V15h2.5a.5.5 0 0 1 0 1h-3a.5.5 0 0 1-.5-.5v-3a.5.5 0 0 1 .5-.5Zm15 0a.5.5 0 0 1 .5.5v3a.5.5 0 0 1-.5.5h-3a.5.5 0 0 1 0-1H15v-2.5a.5.5 0 0 1 .5-.5ZM4 4h1v1H4V4Z"/>
                <path d="M7 2H2v5h5V2ZM3 3h3v3H3V3Zm2 8H4v1h1v-1Z"/>
                <path d="M7 9H2v5h5V9Zm-4 1h3v3H3v-3Zm8-6h1v1h-1V4Z"/>
                <path d="M9 2h5v5H9V2Zm1 1v3h3V3h-3ZM8 8v2h1v1H8v1h2v-2h1v2h1v-1h2v-1h-3V8H8Zm2 2H9V9h1v1Zm4 2h-1v1h-2v1h3v-2Zm-4 2v-1H8v1h2Z"/>
                <path d="M12 9h2V8h-2v1Z"/>
            </svg>
        </button>
    </center>
    
    <!-- Modal -->
        <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
            <div class="modal-header">
                <h1 class="modal-title fs-5     " id="exampleModalLabel">Mire a Câmera do seu celular nesse Qrcode</h1>
                <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
            </div>
            <div class="modal-body">
               <img src="../../../assets/qrcode_exataengenhariapi.com.png" alt="qrcode" class="img-fluid">
            </div>
            <div class="modal-footer">
                <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Fechar</button>
            </div>
            </div>
        </div>
        </div>
</template>


<script>
    import './style/style.css'
</script>

<style>
#container__three {
    position: relative;
}

@media screen and (max-width: 990px) {
    .container__slide {
        margin-top: 10rem;
        height: 110vh !important;
    }
}

#qrcode__icon{
    color: var(--color-green-1);
    text-decoration: none;
    border: none;
}


@media screen and (max-width: 990px) {
    #qrcode__icon {
        position: relative;
        top: 23vh;
    }
}
</style>