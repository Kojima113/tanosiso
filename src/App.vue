<template>
  <div id="app">
    <Top />
    <TabMenu />
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view/>
  </div>
</template>

<script>
import Top from './components/Top.vue'
import TabMenu from './components/TabMenu.vue'

export default {
  components: {
    Top,
    TabMenu
  }
}
</script>


<style>
#app {
  text-align: center;
  background: black;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
