<template>
  <div id="app">
    <SideBar />
    <div class="upper-section-container">
      <NotificationChartContainer />
      <Tasks />
    </div>
    <ClientsMessagesContainer />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import SideBar from './components/SideBar.vue'
import ClientsMessagesContainer from './components/ClientsMessagesContainer.vue'
import NotificationChartContainer from './components/NotificationChartContainer.vue'
import Tasks from './components/Tasks.vue'

@Component({
  components: {
    SideBar,
    ClientsMessagesContainer,
    NotificationChartContainer,
    Tasks,
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

.upper-section-container {
  display: flex;
  flex-direction: row;
}
</style>
