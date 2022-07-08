<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <a class="navbar-item" href="https://bulma.io">
        <img src="./assets/logo.png" alt="">
      </a>

      <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>

    <div id="navbarBasicExample" class="navbar-menu">

      <h1 class="navbar-item">
        Agile Consulting
      </h1>

      <div class="navbar-end">
        <div class="navbar-item">
          <div class="buttons">
            <a class="button is-primary">
              <strong>WhatsApp</strong>
            </a>
            <a class="button is-light">
              Suporte
            </a>
          </div>
        </div>
      </div>
    </div>
  </nav>

  

  <div class="columns">
    <div class="column is-3">
    
      <div class="menuPrincipal">
        <aside class="menu">
          <p class="menu-label">
            Administração
          </p>
          <ul class="menu-list">
            <ul class="menu-list">
              <li>
                <router-link to="/especialidade">Especialidade</router-link>
              </li>
              <li>
                <router-link to="/convenio">Convenio</router-link>
              </li>
            </ul>
          </ul>

          <p class="menu-label">
            Pessoa
          </p>
          <ul class="menu-list">
            <li><a>Medico</a></li>
            <li><a>Paciente </a></li>
            <li><a>Secretaria </a></li>
          </ul>
          <p class="menu-label">
            Agenda
          </p>
          <ul class="menu-list">
            <li><a>Agendamentos</a></li>
            <li><a>Historico</a></li>
          </ul>
        </aside>
      </div>

    </div>
    <div class = "column is-9">
      <router-view />
    </div>
  </div>
</template>

<style lang="scss">
@import "~bulma/bulma.sass";


.navbar {

  background-color: #9ad6bb;
}

.navbar-item img {

  max-height: 3.50rem;
}



#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.menuPrincipal {
  padding: 5rem 3rem;
  background-color: #e0dfdf;
  height: 100vh; 
;
  

  p {
    font-weight: bold;
    color: #9ad6bb;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
