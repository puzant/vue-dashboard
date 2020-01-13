<template>
  <div id="app">
    <SideBar />
    <Notifications />
    <SalesChart />
    <Clients />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import SideBar from './components/SideBar.vue';
import Notifications from './components/Notifications.vue';
import SalesChart from './components/SalesChart.vue';
import Clients from './components/Clients.vue';


@Component({
  components: {
    SideBar,
    Notifications,
    SalesChart,
    Clients
  },
})
export default class App extends Vue {}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #fff;
}
</style>
