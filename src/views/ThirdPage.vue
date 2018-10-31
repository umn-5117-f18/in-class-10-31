<template>
  <div>
    <h1>this is a third page</h1>
    <p>URL path parameter: {{ $route.params.name }}</p>
    <p>URL query parameter: {{ $route.query.a }}</p>
  </div>
</template>
