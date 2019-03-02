<template>
  <v-container fluid>
    <v-layout row wrap justify-center class="mb-5">
      <v-flex xs12>
        <h2 class="primary--text display-2 text-xs-center mb-3">2019 Oscars Volunteer Event</h2>
        <v-divider></v-divider>
      </v-flex>
      <v-flex xs12 md6 xl5 class="pa-3 fw">
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,q_80,w_800/v1551386116/VOWAID/oscars2019.jpg"
          alt="volunteers"
          class="responsive-img elevation-12"
        >
      </v-flex>
      <v-flex xs12 md6 xl5 class="pa-3 fw">
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,w_800/v1551387614/VOWAID/oscars2019-execs.jpg"
          alt="execs"
          class="responsive-img elevation-12"
        >
      </v-flex>
      <v-flex xs12 md6 xl5 class="pa-3 fw">
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,w_800/v1551387614/VOWAID/oscars2019-meeting.jpg"
          alt="meeting"
          class="responsive-img elevation-12"
        >
      </v-flex>
      <v-flex xs12 md6 xl5 class="pa-3 fw">
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,w_800/v1551387614/VOWAID/oscars2019-brief.jpg"
          alt="brief"
          class="responsive-img elevation-12"
        >
      </v-flex>
      <v-flex xs12 md6 xl5 class="pa-3 fw">
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,w_800/v1551387687/VOWAID/oscars2019-alice.jpg"
          alt="prep"
          class="responsive-img elevation-12"
        >
      </v-flex>
      <v-flex xs12 md6 xl5 class="pa-3 fw">
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,w_800/v1551387614/VOWAID/oscars2019-tux.jpg"
          alt="tuxedo"
          class="responsive-img elevation-12"
        >
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "oscars2019"
};
</script>

<style lang="scss" scoped>
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
    font-size: 26px !important;
    margin: 10px auto !important;
  }
}
</style>

