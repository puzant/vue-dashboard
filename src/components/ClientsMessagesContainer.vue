<template lang="pug">
  .clients-messages-container
    Clients
    Messages

</template>


<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'
import Clients from '@/components/Clients.vue';
import Messages from '@/components/Messages.vue';

@Component({
  components: {
    Clients,
    Messages
  }
})
export default class ClientsMessagesContiner extends Vue {

}
</script>

<style lang="sass">
.clients-messages-container
  display: flex
  flex-direction: row
  align-items: center
</style>