<template>
  <v-container fluid class="hero-background-circuit pa-3 wrapper">
    <v-layout wrap justify-center align-center>
      <!-- BLOG POST 1 -->
      <v-flex xs12 md6 lg4>
        <v-card class="elevation-12 ma-3 card">
          <v-img
            src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,w_1000,b_black,o_70/v1549426148/StealthEntry/detected.jpg"
            alt="detected"
            class="white--text"
          >
            <v-container fill-height fluid>
              <v-layout fill-height>
                <v-flex xs12>
                  <span class="display-1">Five Benefits of an MSSP</span>
                </v-flex>
              </v-layout>
            </v-container>
          </v-img>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>
    
<script>
export default {};
</script>

<style lang="scss" scoped>
.wrapper {
  margin: 0;
  padding: 0;
  width: 100vw;
  min-height: 100vh;
}
.hero-background-circuit {
  background-repeat: repeat;
}
/* Mobile Phone Styling */
@media screen and (max-width: 599px) {
  .container {
    padding: 10px !important;
  }
  .card {
    margin: 10px 0 !important;
  }
  .display-1 {
    font-size: 2em !important;
    font-weight: 300 !important;
  }
}
</style>
