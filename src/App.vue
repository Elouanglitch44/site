<template>
  <!-- entete -->
  <header class="navbar-fixeds">
    <nav class="nav-extended  black darken-1 ptm">
      <div class="nav-wrapper mlm">
        <a href="#" class="brand-logo">
          <i class="material-icons">time_to_leave</i>Le transférateur
        </a>
        <a href="#" data-target="slide-out" class="sidenav-trigger">
          <i class="large material-icons">apps</i>
        </a>
        <ul id="nav-mobile" class="right hide-on-med-and-down">
          <li><a href="https://github.com/Elouanglitch44" target="_blank">Elouanglitch44</a></li>
        </ul>
      </div>
      <div class="nav-content">
        <ul class="tabs tabs-transparent">
          
       </ul>
      </div>
    </nav>

    <ul class="sidenav" id="slide-out">
      <li><a href="https://github.com/Elouanglitch44" target="_blank">Elouanglitch44</a></li>
      <img src="./assets/img/Emerie2.jpg">

    
    </ul>

  </header>

  <!-- principale -->
  <main>

    <div class="home" style="margin-top: 2rem">
      <img class="responsive-img circle" alt="Vue logo" src="./assets/img/Nb_lamborghini.jpg">
      <HelloWorld msg="Bienvenue dans ton application Transférateur"/>
    </div>
    
    <div class="row">

      <div class="col s12 m4">
        <div class="card blue-grey darken-1">
          <div class="card-image">
            <img src="./assets/img/Nb_lamborghini.jpg" :class="animate1">
            <span class="card-title">Lamborghini bleue</span>
          </div>
          <div class="card-content white-text">
            <p>C'est une très belle Lamborghini bleue devant une grosse villa à Monaco.
              La Villa a une vue splendide sur la mer ou à coté on peut se balader en Lamborghini.
           </p>
        </div>
          <div class="card-action">
            <a href="#" v-on:click.prevent="animation1()">animer</a>
          </div>
        </div>
      </div>

      <div class="col s12 m4">
        <div class="card blue-grey darken-1">
          <div class="card-image">
            <img src="./assets/img/LamborghiniBla.jpg" :class="animate2">
            <span class="card-title">Lamborghini Blanche</span>
          </div>
          <div class="card-content white-text">
            <p>C'est une très belle Lamborghini blanc devant une grosse Église au Vatican.
              L'Église a une vue splendide sur la ville ou à coté on peut se balader en Lamborghini.
           </p>
          </div>
          <div class="card-action">
            <a href="#" v-on:click.prevent="animation2()">animer</a>
          </div>
        </div>
      </div>
    

       <div class="col s12 m4">
         <div class="card blue-grey darken-1">
           <div class="card-image">
             <img src="./assets/img/MclarenNB.jpg" :class="animate3">
             <span class="card-title">Mclaren</span>
           </div>
           <div class="card-content white-text">
             <p>C'est une très belle Mclaren orange dans un paysage rocheux aux USA .
               Le paysage a une vue splendide sur la plaine Américaine ou à coté on peut se balader en Maclaren .
            </p>
            </div>
           <div class="card-action">
             <a href="#" v-on:click.prevent="animation3()">animer</a>
           </div>
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
          <h5 class="white-text">Le transférateur </h5>
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

img.animated {
  animation: filter-animation 5s 5;
}

@keyframes filter-animation {
  0% {
    filter: sepia(0) saturate(2);
  }

  50% {
    filter: sepia(1) saturate(8);
  }

  100% {
    filter: sepia(0) saturate(2);
  }
}
</style>


<script>


// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'


export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  data: function () {
    return {
      animate1: '',
      animate2: '',
      animate3: ''
    }
  },
  methods: {
    animation1: function () {
      // `this` inside methods point to the Vue instance
      this.animate1 = 'animated'
      this.animate2 = ''
      this.animate3 = ''
    },
    animation2: function () {
      // `this` inside methods point to the Vue instance
      this.animate2 = 'animated'
      this.animate1 = ''
      this.animate3 = ''
    },
    animation3: function () {
      // `this` inside methods point to the Vue instance
      this.animate3 = 'animated'
      this.animate1 = ''
      this.animate2 = ''
    }
  }
}
</script>