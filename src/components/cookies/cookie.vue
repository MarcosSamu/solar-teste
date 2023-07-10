<template>
    <div v-if="!accepted && !declined" class="cookie-consent alert alert-info alert-dismissible fade show m-0" role="alert">
      <p class="mb-0">
        Este site usa cookies para garantir uma melhor experiência para você. Aceita o uso de cookies?
      </p>
      <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Fechar" @click="hideBanner"></button>
      <button type="button" class="btn btn-primary btn-sm mx-2" @click="acceptCookies">Aceitar</button>
      <button type="button" class="btn btn-secondary btn-sm" @click="declineCookies">Recusar</button>
    </div>
  </template>
  
  <script>
  import VueCookies from 'vue-cookies';
  
  export default {
    data() {
      return {
        accepted: false,
        declined: false
      };
    },
    methods: {
      acceptCookies() {
        this.accepted = true;
        VueCookies.set('cookiesAccepted', true, '365d'); // Salva o consentimento do usuário por 365 dias
      },
      declineCookies() {
        this.declined = true;
        VueCookies.remove('cookiesAccepted'); // Remove o consentimento do usuário
        // Outras ações adequadas para remover cookies existentes
      },
      hideBanner() {
        this.accepted = true;
        this.declined = false;
      }
    },
    mounted() {
      const cookiesAccepted = VueCookies.get('cookiesAccepted');
      if (cookiesAccepted) {
        this.accepted = true;
      }
    }
  };
  </script>
  
  <style scoped>
  .cookie-consent {
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    padding: 10px;
    margin-bottom: 0; /* Removendo margem inferior */
    border-top: 1px solid #dee2e6;
    z-index: 1000;
  }
  </style>
  