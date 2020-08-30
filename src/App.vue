<template>
  <div id="app">
    <div id="nav">
      <div class="nav-container">
        <!-- Logo -->
        <div id="logo">
               <router-link to="/"> <img src="./assets/logo.png" alt="logo" /></router-link>
        </div>

        <ul id="icons">
          <li>
            <router-link to="/">Home</router-link>  <i class="fas fa-user"></i>
          </li>
          <li>
            <router-link to="/about">About</router-link> <i class="fa-check"></i>
            <span id="nav-notif"></span>
          </li>
          <li>
            <i class="fas fa-shopping-cart"></i>
          </li>
         </ul>
    </div>
  </div>
<router-view/>

  </div>
</template>

<style lang="scss">


  @import "./assets/css/index.css";
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
