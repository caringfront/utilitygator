<template>
  <div class="white">
     <div>
    <gmap-map
      :center="center"
      :zoom="13"
      style="width:100%; height:100vh">
      <gmap-marker
        :key="id"
        v-for="(m, id) in markers"
        :position="m"
        @click="center=m"
        :clickable="true && false" />
    </gmap-map>
     </div>
  </div>
</template>

<script>

import usersData from '../base/users.json'
export default {
  components: {},
  name: "DrawGoogleMap",
  data() {
    return {
      center: { 
          lat: 30.3961731, 
          lng: -97.7173822
      },
      usersData:[],
      marker:usersData,
      markers: [],
      currentLocation: null
    };
  },
 
  mounted() {
    this.setLocationLatLng();
    this.markers.push()
     
          
  },
 
  methods: {
    setPlace(loc) {
      this.currentLocation = loc;
    },
    setLocationLatLng: function() {
      this.markers= usersData
 
    }
  }
};
</script>