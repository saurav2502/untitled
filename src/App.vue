<template>
  <div id="App">
    <nav>
      <ul>
        <li>
          <router-link to="/Todos">todo</router-link>
        </li>
      </ul>
    </nav>
    <HelloWorld/>
    <Todos/>
  </div>
</template>

<script>
import Todos from "./components/Todos";
//import HelloWorld from "./components/HelloWorld";
export default {
  name: "App",
  components: {
    Todos
    //HelloWorld
  },
  data() {
    return {
      todos: [
        {
          id: 1,
          title: "todo1",
          completed: false
        },
        {
          id: 2,
          title: "todo2",
          completed: false
        },
        {
          id: 3,
          title: "todo3",
          completed: false
        }
      ]
    };
  }
};
</script>

<style scoped>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}

nav li {
  color: #07c;
  text-decoration: underline;
  cursor: pointer;
}
</style> 
