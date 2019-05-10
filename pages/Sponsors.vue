<template>
  <v-container>
    <v-layout row wrap justify-center>
      <v-flex xs12 md10 xl8 class="text-xs-center mb-5">
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/f_auto/v1541276218/VOWAID/darkblade.png"
          alt="darkblade logo"
          class="responsive-img"
        >
        <h6 class="title primary--text mt-3 mb-2">V.I.P. Corporate Sponsor</h6>
        <div data-aos="fade-right" data-aos-delay="200" data-aos-duration="1000">
          <h3 class="display-1 font-weight-regular">Employing Intelligence Community Veterans</h3>
          <p
            class="subheading secondary--text text-xs-left my-3"
          >Darkblade Systems is based in Northern Virginia with personnel supporting Intelligence Community (IC) and Department of Defense (DOD) customers in CONUS and OCONUS locations. Darkblade leadership is comprised of prior military intelligence and special operations personnel with diverse complex operations experience. Many Darkblade employees have served proudly in the U.S. Military, and all continue to support the military and intelligence communities in their civilian efforts.</p>
          <v-btn
            large
            round
            href="https://darkbladesystems.com"
            target="_blank"
            class="primary white--text mb-5"
          >Visit Site</v-btn>
        </div>
      </v-flex>
      <v-flex xs12 md10 xl8 class="text-xs-center mb-5">
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,w_700/v1535434994/codeHunter-shadowed.png"
          alt="codehunter logo"
          class="responsive-img"
        >
        <h6 class="title success--text mt-3 mb-2">Team Member and Volunteer</h6>
        <div data-aos="fade-left" data-aos-delay="200" data-aos-duration="1000">
          <h3 class="display-1 font-weight-regular">Creator of this Website</h3>
          <p
            class="subheading secondary--text text-xs-left my-3"
          >Independent contractor that codes performant, cutting edge websites for small businesses and individuals. In addition to sites, a number of other services are offered, to include: logo design, web hosting, and web consulting on many things related to tech and small businesses. Need someone to handle this part of your business? Get in touch today.</p>
          <v-btn
            large
            round
            href="https://www.codehunter.io"
            target="_blank"
            class="success white--text mb-5"
          >Visit Site</v-btn>
        </div>
      </v-flex>

      <v-flex xs12 md10 lg8 xl6>
        <v-card class="text-xs-center py-3 px-2 nuxtwhite">
          <h3 class="headline">Become a Corporate Sponsor</h3>
          <h5
            class="subheading secondary--text py-2"
          >Please contact our team to discuss our Corporate Sponsor program, and benefits!</h5>
          <v-btn large round to="/contact" class="primary white--text">Get in Touch</v-btn>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "sponsors"
};
</script>

<style lang="scss" scoped>
@media screen and (max-width: 399px) {
  h3.display-1 {
    font-size: 32px !important;
  }
}
</style>
