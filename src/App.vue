<template>
  <div id="app-container" class="container">
    <header class="header">
      <h1>Posts</h1>
    </header>
    <Posts></Posts>
  </div>
</template>

<script>
import Posts from './components/Posts.vue'

export default {
  name: 'App',
  components: {
    Posts
  }
}
</script>

<style>
#app-container {
  margin-top: 60px;
}
h1 {
  text-align: center;
  margin-bottom: 1.5rem;
}
</style>
