<template>
  <!-- entete -->
  <header class="navbar-fixeds">
    <nav class="nav-extended  black darken-1 ptm">
      <div class="nav-wrapper mlm">
        <a href="#" class="brand-logo">
          <i class="material-icons large">blur_on</i>Le transferateur
        </a>
        <a href="#" data-target="slide-out" class="sidenav-trigger">
          <i class="material-icons">menu</i>
        </a>
        <ul id="nav-mobile" class="right hide-on-med-and-down">
          <li><a href="https://github.com/Elouanglitch44" target="_blank">Elouanglitch44</a></li>
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
      <img alt="Vue logo" src="./assets/img/Nb_lamborghini.jpg">
      <HelloWorld msg="Welcome to Your Vue.js App"/>
    </div>

    <div class="row">

      <div class="col s12 m6">
        <div class="card blue-grey darken-1">
          <div class="card-image">
            <img src="./assets/img/Nb_lamborghini.jpg">
            <span class="card-title">Lamborghini bleue</span>
          </div>
          <div class="card-content white-text">
            <p>C'est une très belle Lamborghini bleue devant une grosse villa à Monaco.
              La Villa a une vue splendide sur la mer ou à coté on peut se balader en Lamborghini.
            </p>
          </div>
        </div>
      </div>

      <div class="col s12 m6">
        <div class="card blue-grey darken-1">
          <div class="card-image">
            <img src="./assets/img/LamborghiniBla.jpg">
            <span class="card-title">Lamborghini Blanche</span>
          </div>
          <div class="card-content white-text">
            <p>C'est une très belle Lamborghini blanc devant une grosse Église au Vatican.
              L'Église a une vue splendide sur la place ou à coté on peut se balader en Lamborghini.
            </p>
          </div>
        </div>
      </div>
      
    </div>

<div class="col s12 m6">
        <div class="card blue-grey darken-1">
          <div class="card-image">
            <img src="./assets/img/MclarenNB.jpg">
            <span class="card-title">Mclaren</span>
          </div>
          <div class="card-content white-text">
            <p>C'est une très belle Mclaren orange dans un paysage rocheux aux USA .
              Le paysage a une vue splendide sur l'étendue plaine Américaine ou à coté on peut se balader en Maclaren .
            </p>
          </div>
        </div>
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
          <h5 class="white-text">Le transferateur </h5>
          <p class="grey-text text-lighten-4">Il te sert à aller sur mes informations qui sont importantes.</p>
        </div>
        <div class="col l4 offset-l2 s12">
          <h5 class="white-text">Lien</h5>
          <ul>
            <li><a class="grey-text text-lighten-3" href="https://github.com/Elouanglitch44">Elouanglitch44</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="footer-copyright">
      <div class="container">
        © 2020 Copyright Elouan
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