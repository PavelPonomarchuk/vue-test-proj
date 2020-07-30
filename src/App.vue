<template>
  <div id="app">
    <h1>Какая-то страница</h1>
    <hr>
    <p>Какой-то текст, парам пам пам</p>
    <UnknownError />
  </div>
</template>

<script>
import UnknownError from "@/components/UnknownError";

export default {
  name: 'App',
  components: {
    UnknownError
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
