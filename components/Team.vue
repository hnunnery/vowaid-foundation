<template>
  <v-container fluid>
    <v-layout wrap justify-center align-center class="py-4 row">
      <v-flex xs12 class="mt-3 mb-4">
        <h2 class="display-2 primary--text text-xs-center mb-2">Our Team</h2>
        <v-divider></v-divider>
      </v-flex>
      <!-- Israel Profile -->
      <v-flex xs12 lg6 xl5 class="pa-2 mobile-padding">
        <v-card class="elevation12 pa-3 card">
          <v-layout row wrap justify-center align-center>
            <v-flex xs12 sm5 class="mb-3">
              <v-img
                src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,e_grayscale,f_auto,q_100,w_300/v1534994567/VOWAID/ace.jpg"
                alt="ace"
                height="250px"
                contain
              ></v-img>
            </v-flex>
            <v-flex xs12 sm7 class="text-xs-center">
              <div class="display-2 black--text text--lighten-4 mt-2">Nate Acevedo</div>
              <div class="headline primary--text pt-1 pb-2">Chief Executive Officer</div>
              <div class="secondary--text subheading pt-2 px-3 widen">
                <p>nateacevedo@vowaidfoundation.org</p>
              </div>
            </v-flex>
          </v-layout>
        </v-card>
      </v-flex>
      <!-- Alice Profile -->
      <v-flex xs12 lg6 xl5 class="pa-2 mobile-padding">
        <v-card class="elevation12 pa-3 card">
          <v-layout row wrap justify-center align-center>
            <v-flex xs12 sm5 class="mb-3">
              <v-img
                src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,e_grayscale,f_auto/v1534994567/VOWAID/alice.png"
                alt="alice"
                height="250px"
                contain
              ></v-img>
            </v-flex>
            <v-flex xs12 sm7 class="text-xs-center">
              <div class="display-2 black--text text--lighten-4 mt-2">Ticiane Ward</div>
              <div class="headline primary--text pt-1 pb-2">Founder and CFO</div>
              <div class="secondary--text subheading pt-2 px-3">
                <p>alice@vowaidfoundation.org</p>
              </div>
            </v-flex>
          </v-layout>
        </v-card>
      </v-flex>
      <!-- Liz Profile -->
      <v-flex xs12 lg6 xl5 class="pa-2 mobile-padding">
        <v-card class="elevation12 pa-3 card">
          <v-layout row wrap justify-center align-center>
            <v-flex xs12 sm5 class="mb-3">
              <v-img
                src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,q_100/v1534994567/VOWAID/liz.jpg"
                alt="liz"
                height="250px"
                contain
              ></v-img>
            </v-flex>
            <v-flex xs12 sm7 class="text-xs-center">
              <div class="display-2 black--text text--lighten-4 mt-2">Liz Hensel</div>
              <div class="headline primary--text pt-1 pb-2">Public Affairs Liaison</div>
              <div class="secondary--text subheading pt-2 px-3">
                <p>liz@vowaidfoundation.org</p>
              </div>
            </v-flex>
          </v-layout>
        </v-card>
      </v-flex>
      <!-- Joe Profile -->
      <v-flex xs12 lg6 xl5 class="pa-2 mobile-padding">
        <v-card class="elevation12 pa-3 card">
          <v-layout row wrap justify-center align-center>
            <v-flex xs12 sm5 class="mb-3">
              <v-img
                src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto/v1534994567/VOWAID/joe.jpg"
                alt="joe"
                height="250px"
                contain
              ></v-img>
            </v-flex>
            <v-flex xs12 sm7 class="text-xs-center">
              <div class="display-2 black--text text--lighten-4 mt-2">Joe Caci</div>
              <div class="headline primary--text pt-1 pb-2">President</div>
              <div class="secondary--text subheading pt-2 px-3">
                <p>joecaci@vowaidfoundation.org</p>
              </div>
            </v-flex>
          </v-layout>
        </v-card>
      </v-flex>
      <!-- Lisa Profile -->
      <v-flex xs12 lg6 xl5 class="pa-2 mobile-padding">
        <v-card class="elevation12 pa-3 card">
          <v-layout row wrap justify-center align-center>
            <v-flex xs12 sm5 class="mb-3">
              <v-img
                src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,e_grayscale,f_auto,w_300/v1539741757/VOWAID/lisa.jpg"
                alt="lisa"
                height="250px"
                contain
              ></v-img>
            </v-flex>
            <v-flex xs12 sm7 class="text-xs-center">
              <div class="display-2 black--text text--lighten-4 mt-2">Lisa Hemmie</div>
              <div class="headline primary--text pt-1 pb-2">Volunteer Team Leader</div>
              <div class="secondary--text subheading pt-2 px-3">
                <p>lisa@vowaidfoundation.org</p>
              </div>
            </v-flex>
          </v-layout>
        </v-card>
      </v-flex>
      <!-- Hunter Profile -->
      <v-flex xs12 lg6 xl5 class="pa-2 mobile-padding">
        <v-card class="elevation12 pa-3 card">
          <v-layout row wrap justify-center align-center>
            <v-flex xs12 sm5 class="mb-3">
              <v-img
                src="https://res.cloudinary.com/missionwebdev/image/upload/e_grayscale,f_auto,w_300/v1538693517/VOWAID/hunter.jpg"
                alt="hunter"
                height="250px"
                contain
              ></v-img>
            </v-flex>
            <v-flex xs12 sm7 class="text-xs-center">
              <div class="display-2 black--text text--lighten-4 mt-2">Hunter Nunnery</div>
              <div class="headline primary--text pt-1 pb-2">Web Developer</div>
              <div class="secondary--text subheading pt-2 px-3">
                <p>hunter@vowaidfoundation.org</p>
              </div>
            </v-flex>
          </v-layout>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "Team"
};
</script>

<style lang="scss" scoped>
@media screen and (max-width: 599px) {
  .mobile-padding {
    padding: 0 !important;
    margin-bottom: 20px;
  }
  .widen {
    padding-left: 0px !important;
    padding-right: 0px !important;
  }
}
@media screen and (max-width: 660px) {
  .display-2 {
    font-size: 36px !important;
  }
}
</style>
