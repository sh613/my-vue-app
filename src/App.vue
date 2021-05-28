<template>
  <div id="app">
    <div>
      <Header></Header>
    </div>
    <div class="hello-wrold">
      <img alt="Vue logo" src="./assets/hana.jpg" />
      <div class="hello-wrold__message">
        {{ message }}
      </div>
    </div>
    <TodoList></TodoList>
  </div>
</template>

<script>
import Header from "@/components/header.vue"
import TodoList from "@/components/Todolist.vue"
export default {
  name: "App",
  components: {
    Header,
    TodoList,
  },
  data: function () {
    return {
      message: "単語帳",
    }
  },
  methods: {},
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: bisque;
}
</style>

<style scoped>
.hello-wrold {
  margin-top: 100px;
  text-align: center;
}

.hello-wrold .hello-world__message {
  color: #502c44;
}
</style>
