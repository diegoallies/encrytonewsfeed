<template>
    
<nav class="navbar navbar-light navbar-expand-lg bg-light justify-content-between">
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo03" aria-controls="navbarTogglerDemo03" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <a class="navbar-brand">Encrypto News</a>
  
  <div class="collapse navbar-collapse" id="navbarTogglerDemo03">
  <form class="form-inline">
    <div class="container">

    <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
    <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>

    </div>

  </form>
  </div>
</nav>
<!-- <nav class="navbar navbar-expand-lg navbar-light bg-light">
  
  <a class="navbar-brand" href="#">Encrypto News</a>

  <div class="collapse navbar-collapse" id="navbarTogglerDemo03">
    <form class="form-inline my">
      <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
      <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
    </form>
  </div>
</nav> -->

  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c5050;
  background: #F1f9ec;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

.navbar-brand{
  text-align: left !important;

}

div#navbarTogglerDemo03 {
  flex-flow: row-reverse;
}
</style>
