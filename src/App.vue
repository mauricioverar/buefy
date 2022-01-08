
<template>
  <div id="app">
      <b-navbar>
          <template slot="brand">
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
              <img src="./assets/logo.png" />
            </b-navbar-item> 
          </template>
          <template slot="start">
            <b-navbar-item tag="router-link" :to="{ path: '/' }"> Inicio 
            </b-navbar-item>
            <b-navbar-dropdown label="Productos">
              <b-navbar-item tag="router-link" :to="{ path: '/p/electronica' }">
                Electrónica
              </b-navbar-item>
              <b-navbar-item tag="router-link" :to="{ path: '/p/decoracion' }">
                Decoración
              </b-navbar-item>
              <b-navbar-item tag="router-link" :to="{ path: '/p/computacion' }">
                Computación
              </b-navbar-item>
            </b-navbar-dropdown>
            <b-navbar-item tag="router-link" :to="{ path: '/medios-de-pago' }">
              Medios de pago
            </b-navbar-item>
          </template>
          <template slot="end">
            <b-navbar-item tag="div">
              <div class="buttons">
                <a class="button is-light">
                  <strong>Regístrate</strong>
                </a>
                <a class="button"> Ingresa               
                </a>
              </div>
            </b-navbar-item>
          </template>
      </b-navbar>
      <router-view></router-view>
  </div>
</template>



<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
