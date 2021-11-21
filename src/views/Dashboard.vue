<template>
  <div>
      <v-row>
              <Side />
          <v-col cols="12" xs="12" sm="12" md="12" lg="12" xl="12" class="orange pa-11 lighten-2">
             <h2 class="white--text font-weight-regular mt-2 mb-12"><v-icon class="white--text">mdi-view-dashboard</v-icon>  Workers map</h2>
          </v-col>
      </v-row>
      <v-row no-gutters class="">
          <v-col cols="12" xs="12" sm="12" md="12" lg="12" xl="12">
            <Atlas />
          </v-col>
      </v-row>
  </div>
</template>

<script>
import Atlas from '../components/Atlas.vue'
import Side from '../components/Side.vue'
export default {
  components: { Side, Atlas },

}
</script>

<style>

</style>