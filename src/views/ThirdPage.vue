<template>
  <div>
    <h1>this is a third page</h1>
    <p>URL path parameter: {{ $route.params.name }}</p>
    <p>URL query parameter: {{ $route.query.a }}</p>

    <button @click="$router.push({name: 'home'})">navigate to home</button>
    <br>
    <button @click="$router.push({name: 'third', params: {name: 'qwer1234'}, query: {a: 22}})">navigate fancy</button>
  </div>
</template>
