<template lang="pug">
  .notification-chart-container
    Notifications
    SalesChart
</template>


<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'
import Notifications from '@/components/Notifications.vue';
import SalesChart from '@/components/SalesChart.vue';

@Component({
  components: {
    Notifications,
    SalesChart
  }
})
export default class NotificationContainer extends Vue {

}

</script>

<style lang="sass">
.notification-chart-container
  display: flex 
  flex-direction: column
</style>