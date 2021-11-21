<template>
  <div>
    <Navbar />
    <div id='show_bg_2'>
        <v-row> 
          <v-col cols="12" xs="12" sm="12" md="6" lg="6" xl="6">
            <!-- <v-btn text large dark class="text-capitalize orange  ma-5">Try the App</v-btn> -->
          </v-col>
        </v-row>
        </div>
         <v-row>
          <v-col cols="12" xs="12" sm="12" md="6" lg="6" xl="6">
            <h1 class="text-h3 ma-14 font-weight-regular orange--text">Make an individual worker in the field safer </h1>
          </v-col>
           <v-col cols="12" xs="12" sm="12" md="6" lg="6" xl="6">
            <h1 class="text-h5 ma-14 orange--text">Effectively manage the safety of employees and contractors on the road and at the job site with Utilitygator. 
              Stay connected to operations with real-time tracking and data intelligence.</h1>
          </v-col>
        </v-row>
        <v-row> 
          <v-col cols="12" xs="12" sm="12" md="12" lg="12" xl="12">
            <Parallax />
          </v-col>
        </v-row>
        <v-row class="pa-14"> 
          <v-col cols="12" xs="12" sm="12" md="6" lg="6" xl="6">
            <h2 class="orange--text text--lighten-2">Case study</h2>
            <h1 class="orange--text text-h4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas pariatur quis harum.</h1>
            <h1 class="orange--text text-h5 mt-10">Lorem ipsum dolor sit amet consectetur adipisicing elit. Earum minima repellat est nemo. Dignissimos deserunt laboriosam illo,
               asperiores consequatur blanditiis, numquam repellendus, fugiat veritatis eum nam atque ut sapiente officiis!</h1>
             <p>
         <a href="#"><button class="orange--text mt-5 text-h5">Read more</button></a></p>
          </v-col>

          <v-col cols="12" xs="12" sm="12" md="6" lg="6" xl="6">
            <p class="text-center"><img class="" src="../assets/crane.jpeg" height="400vh"/></p>
          </v-col>
        </v-row>
        <v-row> 
          <v-spacer/>
          <v-col cols="12" xs="7" sm="7" md="7" lg="7" xl="7">
            <h1 class="text-center text-h3 orange--text font-weight-bold">Utility solutions</h1>
          </v-col>
          <v-spacer/>
        </v-row>
       <v-row class="ml-5">
                
                 <v-col cols="12" xs="4" sm="4" md="4" lg="4" xl="4" class="mt-14">
                     <router-link to="/" custom v-slot="{ navigate }">
                     <v-card @click="navigate" role="link" class="" width="28vw" height="80vh">
                         <img class="" :src="require('../assets/steering.svg')"/>
                          <h2 class="text-h4 ma-4 font-weight-regular orange--text"> Promote driver safety</h2>
                          <h1 class="text-h6 ma-4 font-weight-regular orange--text mt-5">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nihil commodi expedita facilis consectetur el.</h1>
                         <v-btn text to="#" active-class="active" exact class="orange--text btn-link text-capitalize text-h5" x-large>see solution</v-btn>
                     </v-card>
                     </router-link>
                 </v-col>    
                 <v-col cols="12" xs="4" sm="4" md="4" lg="4" xl="4" class="mt-14">
                     <router-link to="/" custom v-slot="{ navigate }">
                     <v-card @click="navigate" role="link" class="" width="28vw" height="80vh">
                         <img class="" :src="require('../assets/magnify.svg')"/>
                          <h2 class="text-h4 ma-4 font-weight-regular orange--text">Monitor worker safety</h2>
                          <h1 class="text-h6 ma-4 font-weight-regular orange--text mt-5">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nihil commodi expedita facilis consectetur el.</h1>
                         <v-btn text to="#" active-class="active" exact class="orange--text btn-link text-capitalize text-h5" x-large>see solution</v-btn>
                     </v-card>
                     </router-link>
                 </v-col>    

                 <v-col cols="12" xs="4" sm="4" md="4" lg="4" xl="4" class="mt-14">
                     <router-link to="/" custom v-slot="{ navigate }">
                     <v-card @click="navigate" role="link" class="" width="28vw" height="80vh">
                         <img class="" :src="require('../assets/location.svg')"/>
                          <h2 class="text-h4 ma-4 font-weight-regular orange--text">Live tracking</h2>
                          <h1 class="text-h6 ma-4 font-weight-regular orange--text mt-5">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nihil commodi expedita facilis consectetur el.</h1>
                         <v-btn text to="#" active-class="active" exact class="orange--text btn-link text-capitalize text-h5" x-large>see solution</v-btn>
                     </v-card>
                     </router-link>
                 </v-col>                 
             </v-row>
      </div>
</template>

<script>
import Navbar from '../components/Navbar.vue'
import Parallax from '../components/Parallax.vue'
export default {
  components: { Navbar, Parallax },

}
</script>

<style>
#show_bg_2 {
    background-image:
    linear-gradient(to left, rgba(233, 191, 101, 0), rgba(168, 85, 18, 0.73)),
    url('../assets/showcase.jpg');
    height: 80vh;
    background-size: cover;
    color: white;
    padding: 20px;
}
</style>