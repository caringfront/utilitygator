<template>
<div>
    <v-tabs
      v-model="tab"
      background-color="transparent"
    >
      <v-tab>
       Workers
      </v-tab>
       <v-tab>
       Devices
      </v-tab>
       <v-tab>
       Hubs
      </v-tab>
       <router-link to="/logs" custom v-slot="{ navigate }">
       <v-tab @click="navigate" role="link">
       Chatbot Logs
      </v-tab>
      </router-link>
       <v-tab>
       Push-to-talk Events
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item class="">
         <Workers />
      </v-tab-item>
      <v-tab-item class="">
        <devices />
      </v-tab-item>
      <v-tab-item class="">
        Hubs
      </v-tab-item>
       <v-tab-item  class="">
        Chatbot Logs
      </v-tab-item>
       <v-tab-item class="">
        Push-to-talk
      </v-tab-item>
    </v-tabs-items>
</div>
</template>
<script>
import Devices from './Tabs/Devices.vue'
import Workers from './Tabs/Workers.vue'
// 
  export default {
  components: {Workers, Devices  },
    data () {
      return {
        tab: null,
      }
    },
  }
</script>