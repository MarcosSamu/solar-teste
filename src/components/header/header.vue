<template>
  <nav :class="navbarClass" class="navbar navbar-expand-lg bg-body-tertiary fixed-top">
    <div class="container-fluid header__elements">
      <a class="navbar-brand" href="#">
        <img src="../../assets/logo.png" width="150" alt="Logo Solar Vistoria">
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarSupportedContent">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#servicos">Serviços</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#sobre">Sobre</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#baixe">Baixe nosso App</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#contato">Contato</a>
          </li>
          <li class="nav-item">
            <a class="button__login btn" href="https://alfaweb.meugestorsolar.com" target="_blank">Login</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <Banner />
</template>

<script>
import Banner from '../banner/banner.vue'
import './styles/style.css'

export default {
  components: {
    Banner,
  },
  data() {
    return {
      scrollPosition: 0
    }
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll)
  },
  methods: {
    handleScroll() {
      this.scrollPosition = window.pageYOffset
    }
  },
  computed: {
    navbarClass() {
      return {
        'navbar-with-shadow': this.scrollPosition >= 500
      }
    }
  }
}
</script>

<style scoped>
.nav-link {
  color: var(--color-black-1);
  font-weight: 400;
  font-size: 1rem;
  margin: 0 16px;
}

.nav-link:hover {
  color: var(--color-green-1);
}

.header__elements {
  padding: 0 152px;
}

.button__login {
  background-color: var(--color-green-1);
  border-radius: 0;
  color: var(--color-white-1);
}



.navbar-with-shadow {
  box-shadow: 0 2px 4px  2px rgba(0, 0, 0, 0.2);
}
</style>
