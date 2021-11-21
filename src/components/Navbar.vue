<template>
  <div>
      <v-app-bar class="white" height="100vh" flat app>
        <router-link to="/" custom v-slot="{ navigate }">
       <img @click="navigate" role="link" class="" :src="require('../assets/utilitygator_logo.png')" height="60"/>
       </router-link>
       <v-spacer />
       <v-btn text class="orange--text text-h6 font-weight-regular text-capitalize">Home</v-btn>
       <v-btn text class="orange--text text-h6 font-weight-regular text-capitalize">Products</v-btn>
       <v-btn text class="orange--text text-h6 font-weight-regular text-capitalize">Solutions</v-btn>
       <v-btn text class="orange--text text-h6 font-weight-regular text-capitalize">Resources</v-btn>
       <v-btn text class="orange--text text-h6 font-weight-regular text-capitalize">Blog</v-btn>
       <v-btn text class="orange--text text-h6 font-weight-regular text-capitalize">Contact</v-btn>
      
       <v-spacer />
         <v-btn to="/dashboard" text large dark class="text-capitalize orange  ma-5">Try the App</v-btn>
         <v-btn to="/login" class="orange--text" outlined large>login</v-btn>
      </v-app-bar>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>