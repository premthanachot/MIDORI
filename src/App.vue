<template>
  <div id="app">
    <div id="app1">
      <b-navbar toggleable type="dark" variant="dark" fixed="top">
        <b-navbar-brand href="/">Midori Shop</b-navbar-brand>

        <b-navbar-toggle target="navbar-toggle-collapse">
          <template #default="{ expanded }">
            <b-icon v-if="expanded" icon="chevron-bar-up"></b-icon>
            <b-icon v-else icon="chevron-bar-down"></b-icon>
          </template>
        </b-navbar-toggle>

        <b-collapse id="navbar-toggle-collapse" is-nav>
          <b-navbar-nav class="ml-auto">
            <b-nav-item href="/"
              ><b-icon icon="house"></b-icon> Home</b-nav-item
            >
            <b-nav-item href="/about"
              ><b-icon icon="person-circle"></b-icon> Profile</b-nav-item
            >
            <b-nav-item href="/login"
              ><b-icon icon="power"></b-icon> Login</b-nav-item
            >
            <b-nav-item href="/product"
              ><b-icon icon="box"></b-icon> Product</b-nav-item
            >
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
    <router-view />
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
#app1 {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
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
