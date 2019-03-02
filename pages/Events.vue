<template>
  <v-container fluid>
    <v-layout row wrap justify-center class="mb-5">
      <v-flex xs12 md6 xl5 class="pa-5 fw text-xs-center">
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,q_80,w_800/v1551386116/VOWAID/oscars2019.jpg"
          alt="volunteers"
          class="responsive-img elevation-12 mb-3"
        >
        <h2 class="mt-3 twentyeight primary--text">2019 Oscars Volunteer Event</h2>
        <v-divider class="mb-2"></v-divider>
        <p
          class="subheading secondary--text text-xs-left"
        >VOWAID raised eleven thousand dollars by providing Safety Ambassadors for the 2019 OSCARS. All of our volunteers are active duty and Veterans! United for a change! Raised funds are going towards helping Veterans in need.</p>
        <v-btn to="/oscars19" class="primary white--text">See More</v-btn>
      </v-flex>
      <v-flex xs12 md6 xl5 class="pa-5 fw text-xs-center">
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,w_1440/v1538694547/VOWAID/coachella.jpg"
          alt="concert"
          class="responsive-img elevation-12 mb-3"
        >
        <h2 class="mt-3 twentyeight primary--text">2018 Coachella Volunteer Event</h2>
        <v-divider class="mb-2"></v-divider>
        <p
          class="subheading secondary--text text-xs-left"
        >VOWAID raised 22 thousand dollars by serving as Safety Ambassadors for Coachella. Our Volunteers had a lot of fun securing the VIP areas and ensuring everyone's safety. Proceeds were used to help Veteran families.</p>
      </v-flex>
      <v-flex xs12 md6 xl5 class="pa-5 fw text-xs-center">
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,q_auto:best,w_1440/v1535518449/VOWAID/oscarsedit.jpg"
          alt="group photo"
          class="responsive-img elevation-12 mb-3"
        >
        <h2 class="mt-3 twentyeight primary--text">2018 Oscars Volunteer Event</h2>
        <v-divider class="mb-2"></v-divider>
        <p
          class="subheading secondary--text text-xs-left"
        >VOWAID raised nine thousand dollars by providing Safety Ambassadors for the 2018 OSCARS. All of our volunteers are active duty and Veterans! United for a change! Raised funds are going towards helping Veterans in need.</p>
      </v-flex>
      <v-flex xs12 sm8 xl7 class="mx-2">
        <v-card class="pa-3">
          <v-layout row wrap justify-center align-center class="text-xs-center">
            <v-flex xs12>
              <h2 class="twentyeight primary--text">Volunteer Waiver Forms</h2>
              <v-divider class="mb-2"></v-divider>
            </v-flex>
            <v-flex xs12 md6 class="text-xs-center my-3">
              <v-btn large class="primary white--text">
                <a href="/waiver1.pdf" download>Download Waiver Form 1</a>
              </v-btn>
            </v-flex>
            <v-flex xs12 md6 class="text-xs-center">
              <v-btn large class="primary white--text">
                <a href="/waiver2.pdf" download>Download Waiver Form 2</a>
              </v-btn>
            </v-flex>
          </v-layout>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "services"
};
</script>

<style lang="scss" scoped>
.container {
  padding-top: 0;
}
@media screen and (max-width: 599px) {
  .container,
  .fw {
    padding: 0 0 50px 0 !important;
    margin: 0 !important;
  }
  h2,
  p {
    padding: 0 10px;
  }
  h2 {
    font-size: 24px !important;
    margin: 10px auto !important;
  }
}
</style>

