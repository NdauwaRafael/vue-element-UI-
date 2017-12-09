<template>
  <div id="app">
    <topbar></topbar>
    <addsite></addsite>
    <appfooter></appfooter>
  </div>
</template>

<script>
import topbar from './components/topbar.vue';
import appfooter from './components/footer.vue'
import addsite from './components/addsite.vue'
import TabBar from "../node_modules/element-ui/packages/tabs/src/tab-bar.vue";
export  default {
    components: {topbar, appfooter, addsite}
}
</script>

<style>
#app {
  font-family: Helvetica, sans-serif;
  text-align: center;
}
</style>
