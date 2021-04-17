<template>
 <div id="app">
   <h1>ToDo App</h1>
   <hr>
   <ToDoList v-bind : todos="todos"/>
 </div>

</template>

<script>
import ToDoList from "@/components/ToDoList"
export default {
  name: 'App',
  data(){
    return{
      todos: [
        {id: 1, text: "Do the dishes", completed: "false"},
        {id: 2, text: "Do the laundry", completed: "false"},
        {id: 3, text: "Fix a meal", completed: "false"}
      ]
    }
  },
  components: {
    ToDoList : ToDoList
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
