<template>
  <nav class="navbar navbar-expand-lg bg-light">
  <div class="container-fluid">
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-4">
        <li class="nav-item">
          <router-link class="nav-link" to="/">Home</router-link>
        </li>
        
        <li>
          <div class="dropdown">
            <button class="btn btn-success dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
              Artworks
            </button>
            <ul class="dropdown-menu">
              <li class="dropdown-item"><router-link to="/artworks"> Paintings</router-link></li>
              <li class="dropdown-item"><router-link to="/artworks">Drawings</router-link></li>
              <li class="dropdown-item"><router-link to="/artworks">Sculptures</router-link></li>
              <li class="dropdown-item"><router-link to="/artworks">Watercolor Paintings</router-link></li>
            </ul>
          </div>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" to="/signup">SignUp</router-link>
        </li>

        <li class="nav-item">
          <router-link class="nav-link" to="/login">Login</router-link>
        </li>

        <li class="nav-item">
          <router-link class="nav-link" to="/cart">ShippingCart</router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" to="/contact">Contact</router-link>
        </li>

      </ul>
    </div>
  </div>
</nav>

  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 50px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
