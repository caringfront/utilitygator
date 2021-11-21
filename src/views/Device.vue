<template>
  <div>
      <v-row>
              <Side />
          <v-col cols="12" xs="12" sm="12" md="12" lg="12" xl="12" class="orange pa-13 lighten-2">
              <v-row>
             <v-avatar class="grey white--text mt-1 mb-9">{{workers[$route.params.id-1].deviceAvatar}}</v-avatar><h2 class="ml-3 white--text font-weight-regular mt-3">{{workers[$route.params.id-1].device}}</h2>
             </v-row>
          </v-col>
      </v-row>
      <v-row class="pa-3">
          <v-col cols="12" xs="12" sm="12" md="12" lg="12" xl="12" class="pa-5">
            <v-card class="green">
                <v-card-title class="white--text text-h6">Coordinates</v-card-title>
                <Atlas2 />
            </v-card>
          </v-col>
      </v-row>
      <v-row class="pa-3">
          <v-col cols="12" xs="4" sm="4" md="4" lg="4" xl="4" class="pa-5">
            <v-card class="blue">
                <v-card-title class="white--text text-h6">Battery</v-card-title>
                <div class="grey lighten-3 pa-11">
                <p class="text-center"><img style="opacity:50%" class="" :src="require('../assets/battery.png')" height="120"/></p>
                </div>
            </v-card>
          </v-col>

          <v-col cols="12" xs="4" sm="4" md="4" lg="4" xl="4" class="pa-5">
            <v-card class="purple lighten-2">
                <v-card-title class="white--text text-h6">Network</v-card-title>
                 <div class="grey lighten-3 pa-11">
                <p class="text-center"><img style="opacity:50%" class="" :src="require('../assets/wifi.png')" height="120"/></p>
                </div>
            </v-card>
          </v-col>

          <v-col cols="12" xs="4" sm="4" md="4" lg="4" xl="4" class="pa-5">
            <v-card class="grey darken-3">
                <v-card-title class="white--text text-h6">Location</v-card-title>
                 <div class="grey lighten-3 pa-11">
                <p class="text-center"><img style="opacity:50%" class="" :src="require('../assets/marker.png')" height="120"/></p>
                </div>
            </v-card>
          </v-col>
      </v-row>
       <v-row class="pa-3">
          <v-col cols="12" xs="12" sm="12" md="12" lg="12" xl="12" class="pa-5">
            <v-card class="blue darken-3">
                <v-card-title class="white--text text-h6">Alerts</v-card-title>
                <div class="grey lighten-3 pa-11">
                <p class="text-center"><img style="opacity:50%" class="" :src="require('../assets/notify.png')" height="120"/></p>
                </div>
            </v-card>
          </v-col>
      </v-row>
  </div>
</template>

<script>
import workersData from "../Testdata/workers.json"
import Atlas2 from '../components/Atlas2.vue'
import Side from '../components/Side.vue'
export default {
  components: { Side, Atlas2},
    data: () => ({
        workers: workersData,
    }),
}
</script>

<style>

</style>