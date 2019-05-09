<template>
  <v-container fluid class="page-header-image">
    <v-layout row wrap align-center justify-center class="mt-5">
      <v-flex xs12 md8 lg6 xl5 class="text-xs-center">
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,q_100,w_705/v1535429145/VOWAID/vowaid-logo-dark-shadow.png"
          alt="logo"
          class="responsive-img main-logo"
        >
      </v-flex>
      <v-flex xs12 md10 lg6 xl5 class="px-5">
        <div class="hide-on-mobile">
          <h1 class="display-3 font-weight-bold white--text text-xs-center">Mission Statement</h1>
          <h4
            class="headline font-weight-light white--text text-xs-center px-2"
            style="text-shadow: white 1px 1px 3px;"
          >The Veterans of War Aid Foundation (VOWAID) is a 501 (c) 3 non-profit organization founded by U.S. Service Members, dedicated to assisting veterans, spouses and children of disabled veterans, and fallen heroes by providing opportunities for financial, emotional growth, and self-empowerment.</h4>
        </div>
        <br>
        <v-layout row wrap justify-center align-center>
          <v-flex xs3 sm1 class="text-xs-center mt-3">
            <a href="https://twitter.com/vow_aid" target="_blank">
              <v-icon class="white--text" size="32px">fab fa-twitter</v-icon>
            </a>
          </v-flex>
          <v-flex xs3 sm1 class="text-xs-center mt-3">
            <a href="https://www.facebook.com/vowaid" target="_blank">
              <v-icon class="white--text" size="32px">fab fa-facebook-square</v-icon>
            </a>
          </v-flex>
          <v-flex xs3 sm1 class="text-xs-center mt-3">
            <a href="https://www.instagram.com/vow_aid" target="_blank">
              <v-icon class="white--text" size="32px">fab fa-instagram</v-icon>
            </a>
          </v-flex>
          <v-flex xs9 sm4 class="text-xs-center mt-3">
            <v-btn
              large
              round
              to="/store"
              class="primary white--text"
              style="font-size: 1.2rem;"
            >Donate Now</v-btn>
          </v-flex>
        </v-layout>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "hero",
  data() {
    return {};
  }
};
</script>

<style lang="scss" scoped>
.hide-on-mobile {
  @media only screen and (max-width: 450px) {
    display: none;
  }
}
.page-header-image {
  min-height: 100vh;
  background-image: url("https://res.cloudinary.com/missionwebdev/image/upload/c_scale,e_grayscale,f_auto,q_49,w_1200/v1551844806/VOWAID/marine.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
.main-logo {
  max-height: 60vh;
}
</style>