<template>
  <!-- entete -->
  <header class="navbar-fixeds">
    <nav class="nav-extended  black darken-1 ptm">
      <div class="nav-wrapper mlm">
        <a href="#" class="brand-logo">
          <i class="material-icons large">blur_on</i>ELOUAN
        </a>
        <a href="#" data-target="slide-out" class="sidenav-trigger">
          <i class="material-icons">menu</i>
        </a>
        <ul id="nav-mobile" class="right hide-on-med-and-down">
          <li><a href="/" target="_blank">@github</a></li>
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

  </header>

  <!-- principale -->
  <main>

    <div class="home">
      <img alt="Vue logo" src="./assets/logo.png">
      <HelloWorld msg="Welcome to Your Vue.js App"/>
    </div>

  </main>


  <!-- informations -->
  <aside>
  </aside>


  <!-- pied de page -->
  <footer class="page-footer black">
    <div class="container">
      <div class="row">
        <div class="col l6 s12">
          <h5 class="white-text">Footer Content</h5>
          <p class="grey-text text-lighten-4">You can use rows and columns here to organize your footer content.</p>
        </div>
        <div class="col l4 offset-l2 s12">
          <h5 class="white-text">Links</h5>
          <ul>
            <li><a class="grey-text text-lighten-3" href="#!">Link 1</a></li>
            <li><a class="grey-text text-lighten-3" href="#!">Link 2</a></li>
            <li><a class="grey-text text-lighten-3" href="#!">Link 3</a></li>
            <li><a class="grey-text text-lighten-3" href="#!">Link 4</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="footer-copyright">
      <div class="container">
        © 2020 Copyright Text
        <a class="grey-text text-lighten-4 right" href="#!">More Links</a>
      </div>
    </div>
  </footer>

 
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


<script>


// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'


export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>