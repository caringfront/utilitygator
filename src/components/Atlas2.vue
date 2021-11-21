<template>
  <div class="white">
     <div>
    <gmap-map
      :center="center"
      :zoom="11"
      style="width:100%; height:30vh">
      <gmap-marker
        :position="center" />
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