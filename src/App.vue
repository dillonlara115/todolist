<template>
   <div id="app">
      <todo-list v-bind:todos="todos"></todo-list>
   </div>
</template>

<script>
import TodoList from './components/TodoList';

export default {
   name: 'App',
   components: {
      TodoList,
   },
   data() {
      return {
         todos: [{
            tite: 'Todo A',
            project: 'Project A',
            done: false,
         }, {
            tite: 'Todo b',
            project: 'Project b',
            done: true,
         }, {
            tite: 'Todo c',
            project: 'Project c',
            done: true,
         }, {
            tite: 'Todo D',
            project: 'Project D',
            done: false,
         }],
      };
   },
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
