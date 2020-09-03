<template>
  <div id="app">
    <div id="nav">
      <b-navbar toggleable type="dark" class="navbar navbar-expand-lg fixed-top" style="background:#FFF">        
        <div class="container">
            <b-navbar-toggle>
                <i class="fas fa-bars" v-b-toggle.sidebar-no-header style="font-size:1.50rem; color:#000;"></i>
                <b-sidebar id="sidebar-no-header" aria-labelledby="sidebar-no-header-title" no-header shadow>
                <template v-slot:default="{ hide }">                    
                    <div class="p-5">
                        <i class="far fa-times-circle" variant="primary" block @click="hide" style="font-size:2rem;display:flex;"></i>
                        <nav class="mb-8">
                            <b-nav vertical>
                                <b-nav-item to="/">Home</b-nav-item>
                                <b-nav-item to="/servicios">Servicios</b-nav-item>
                                <b-nav-item to="/contacto">Contacto</b-nav-item>
                            </b-nav>
                        </nav>
                    </div>
                </template>
                </b-sidebar>
            </b-navbar-toggle>
            <b-navbar-brand aling="center">
                <router-link to="/">
                  <img src="./assets/logo.png" alt="logo" style="width:5rem;height:5rem;">
                </router-link>           
            </b-navbar-brand>

            <b-collapse id="sidebar-1" is-nav>
                <b-navbar-nav class="ml-auto" >
                  <b-nav-item to="/">Home</b-nav-item>
                  <b-nav-item to="/servicios">Servicios</b-nav-item>
                  <b-nav-item to="/contacto">Contacto</b-nav-item>
                </b-navbar-nav>
            </b-collapse>
        </div>
    </b-navbar>
    </div>
    <router-view/>
    <footer>
      <div class="container">
        <h5><i class="fas fa-copyright"></i> Key Data 2020. Todos los derechos reservados</h5>
      </div>
    </footer>
  </div>
</template>

<style>
*{
  font-family: "Raleway";
}

#app {
  font-family: "Raleway";
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

#nav {
  padding: 30px;
  background: #FFF;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
  font-size: 1.10rem;
}

#nav a.router-link-exact-active {
  color: #11998e;
}

footer{
  background: #1C1D21;
  margin: 0;
  color: #F1F1F1;
  padding: 1rem;
}

footer h5{
  font-size: 1rem;
  text-align: center;
}
</style>
