<template>
  <div>
      <v-row no-gutters>
          <v-col cols="12" xs="7" sm="7" md="7" lg="7" xl="7" class="" id="show_bg_3">
              <h1 class="white--text text-h2">Monitor Your</h1>
              <h1 class="white--text text-h2 mt-5">Workers.</h1>
          </v-col>
           <v-col cols="12" xs="5" sm="5" md="5" lg="5" xl="5" class="pa-14">
               <h1 class="text-center orange--text mt-14">Sign In</h1>
               <h3 class="text-center font-weight-regular">Simply type below the credentials which you received in your email</h3>
               <form action="" class="mt-14">
                <v-text-field placeholder="Email Address"></v-text-field>
                <v-text-field placeholder="Password"></v-text-field>
                <v-btn width="35vw" to="/dashboard" text rounded class="text-capitalize orange" dark>Log in</v-btn>
               </form>
          </v-col>
      </v-row>
  </div>
</template>

<script>
export default {

}
</script>

<style>
#show_bg_3 {
    background-image:
    linear-gradient( rgba(255, 115, 0, 0.884), rgba(255, 115, 0, 0.74)),
    url('../assets/showcase.jpg');
    height: 100vh;
    background-size: cover;
    color: white;
    padding: 200px;
    padding-top: 300px;
}
</style>