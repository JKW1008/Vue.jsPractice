<script>
import TodoInput from "@/components/TodoInput.vue";
import TodoList from "@/components/TodoList.vue";
import { v4 as uuidv4 } from "uuid";

export default {
  data() {
    return {
      todoList: [],
    };
  },
  components: {
    TodoInput,
    TodoList,
  },
  methods: {
    todoInput(msg) {
      const item = {
        id: uuidv4(),
        msg: msg,
        completed: false,
      };
      // console.log(item);
      this.todoList.push(item);
      console.log(JSON.stringify(this.todoList));
    },
  },
};
</script>
<template>
  <div class="todo-container">
    <h1>TODO List</h1>
    <TodoInput @todo-input="todoInput" />
    <TodoList />
  </div>
</template>
