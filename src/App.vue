<template>
<!--  <BaseTemp v-for="post in posts"-->
<!--            :key="posts.indexOf(post)"-->
<!--            :ti="post">占位符</BaseTemp>-->
<!--  <board-box :form="person"></board-box>-->
  <ToList></ToList>
</template>

<script>
import ToList from "@/components/todo/ToList";

export default {
  name: 'App',
  data(){
    return {
      posts: ["标题1", "标题2"],
      person: {
        name: "aaa",
        age: 18
      }
    }
  },
  components: {
    ToList
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
