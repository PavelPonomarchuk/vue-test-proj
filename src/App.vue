<template>
  <div id="app">
    <SomePage />
    <UnknownError />
  </div>
</template>

<script>
import UnknownError from "@/components/UnknownError";
import SomePage from "@/components/SomePage";

export default {
  name: 'App',
  components: {
    UnknownError,
    SomePage
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
