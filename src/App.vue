<template>
  <MainCard />
  <projectCard />
</template>

<script>
import MainCard from './components/MainCard.vue'
import projectCard from './components/ProjectsCard.vue'

export default {
  name: 'App',
  components: {
    MainCard,
    projectCard
  }
}
</script>

<style>
body{
  margin: 20px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #d6edff;
}
</style>
