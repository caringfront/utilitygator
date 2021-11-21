<template>
  <div>
      <v-row>
              <Side />
          <v-col cols="12" xs="12" sm="12" md="12" lg="12" xl="12" class="orange pa-11 lighten-2">
             <h2 class="white--text font-weight-regular mt-1 mb-10"><v-icon class="white--text">mdi-view-dashboard</v-icon> Chat-Bot-Logs</h2>
          </v-col>
      </v-row>
      <v-row class="">
          <v-col cols="12" xs="12" sm="12" md="12" lg="12" xl="12" class="pa-14">
            <Log class="ma-2" />
          </v-col>
      </v-row>
  </div>
</template>

<script>
import Log from '../components/Log.vue'

import Side from '../components/Side.vue'
export default {
  components: { Side, Log },

}
</script>

<style>

</style>