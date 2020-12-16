<template>

  <div class="navbar-fixeds">
    <nav class="nav-extended  black darken-1 ptm">
      <div class="nav-wrapper mlm">
        <a href="#" class="brand-logo">
          <i class="material-icons large">blur_on</i>ADMIN
        </a>
        <a href="#" data-target="slide-out" class="sidenav-trigger">
          <i class="material-icons">menu</i>
        </a>
        <ul id="nav-mobile" class="right hide-on-med-and-down">
          <li><a href="/" target="_blank">EPYO VISIO</a></li>
        </ul>
      </div>
      <div class="nav-content">
        <ul class="tabs tabs-transparent">
          <li class="tab"><a href="#section1">CONFIGURATION</a></li>
          <li class="tab"><a href="#section2">PARAMS</a></li>
          <li class="tab"><a href="#section3">INFORMATIONS</a></li>
          <li class="tab"><a href="#section4">LOGS</a></li>
        </ul>
      </div>
    </nav>

    <ul class="sidenav" id="slide-out">
      <li><a href="/">EPYO</a></li>
    </ul>
  </div>

  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div>
  <router-view/>
</template>

<style lang="scss">

@import "./assets/style.scss";

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
