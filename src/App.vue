<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> | 
      <router-link to="/third/foo">Third Page</router-link>&nbsp;
      <router-link to="/third/bar?a=hello">(1)</router-link>, 
      <router-link to="/third/1-2-3 foo?a=1">(2)</router-link>,
      <router-link :to="{name: 'third', params: {name: 'param-name'}, query: {a: 777}}">(3)</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;

  padding: 30px;
}
#nav {
  margin-bottom: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
