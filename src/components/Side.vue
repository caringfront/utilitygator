<template>
  <div>
   
      <v-navigation-drawer
        permanent
       width="25vw"
       app
       nav 
      >
        <v-list>
          <div class="orange lighten-2">
            <v-row class="pa-10">
          <router-link to="/dashboard" custom v-slot="{ navigate }">
       <img @click="navigate" role="link" class="" :src="require('../assets/electricgator_logo.png')" height="45"/>
       </router-link>
       <v-spacer />
       <v-btn icon><v-icon>mdi-magnify</v-icon></v-btn>
       <v-btn icon><v-icon>mdi-dots-vertical</v-icon></v-btn>
       </v-row>
       <v-row no-gutters>
         <v-col cols="12" xs="12" sm="12" md="12" lg="12" xl="12">
           <Tabs />
         </v-col>
       </v-row>
        </div>
         <!-- <router-link to="/" custom v-slot="{ navigate }">
          <v-list-item @click="navigate" role="link" link>
            <v-list-item-icon>
              <v-icon>mdi-home</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item>
          </router-link>
         
            <router-link to="/" custom v-slot="{ navigate }">
          <v-list-item @click="navigate" role="link" link>
            <v-list-item-icon>
              <v-icon>mdi-chart-bar</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Analytics</v-list-item-title>
          </v-list-item>
           </router-link>
         
              <router-link to="/" custom v-slot="{ navigate }">
          <v-list-item @click="navigate" role="link" link>
            <v-list-item-icon>
              <v-icon>mdi-video</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Live</v-list-item-title>
          </v-list-item>
             </router-link>
         
              <router-link to="/" custom v-slot="{ navigate }">
           <v-list-item @click="navigate" role="link" link>
            <v-list-item-icon>
              <v-icon>mdi-account-circle-outline</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Account</v-list-item-title>
          </v-list-item>
             </router-link> -->
        </v-list>
      </v-navigation-drawer>
    
  </div>
</template>

<script>
import Tabs from './Tabs.vue'
export default {
  components: { Tabs },
  
}
</script>

<style>

</style>