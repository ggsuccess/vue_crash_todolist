<template>
  <div id="app">
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>
import Todos from './components/Todos';

export default {
  name: 'app',
  components: {
    Todos
  },
  data() {
    return {
      todos: [
        {
          id: 1,
          title: 'vue.js',
          completed: false
        },
        {
          id: 2,
          title: 'react.js',
          completed: true
        },
        {
          id: 3,
          title: 'angular.js',
          completed: false
        }
      ]
    };
  }
};
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}
</style>
