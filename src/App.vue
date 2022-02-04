<template>
  <div id="app">
    <Top />
    <TabMenu />
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import Top from './components/Top.vue'
import TabMenu from './components/TabMenu.vue'

export default {
  name: 'App',
  components: {
    //HelloWorld,
    Top,
    TabMenu
  }
}
</script>

<style>
#app {
  text-align: center;
  background: black;
  height: 2000px;
}
</style>
