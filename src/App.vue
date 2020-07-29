<template>
  <div id="app">
    <h1>Какая-то страница</h1>
    <hr>
    <TodoList />
    <UnknownError />


  </div>
</template>

<script>
import TodoList from '@/components/TodoList'
import UnknownError from '@/components/UnknownError'

export default {
  name: 'App',
  components: {
    TodoList,
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
