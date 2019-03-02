<template>
  <v-container fluid>
    <v-layout row wrap justify-center class="mb-5">
      <v-flex xs12 md6 xl5 class="pa-5 fw">
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,q_70,w_800/v1546288462/VOWAID/bg29.jpg"
          alt="suit"
          class="responsive-img elevation-12 mb-3"
        >
        <h2 class="text-xs-center mt-3 twentyeight primary--text">Transition Assistance Resources</h2>
        <v-divider class="mb-2"></v-divider>
        <p
          class="subheading secondary--text"
        >The VOWAID TWS provides a personal assistance team that focuses on you (our Veteran client) and your family. We are dedicated to finding state and national resources that will help you readjust to civilian life. We can help you apply for unemployment, find non-profits and local groups that will connect you with a solid support system that will help you through your transition. Our case managers are seasoned Veterans and military spouses who understand the struggles of leaving the service. We also advocate for you during difficult times and situations. We make the tough phone calls so you have the time to focus on what matters.</p>
      </v-flex>
      <v-flex xs12 md6 xl5 class="pa-5 fw">
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,q_70,w_800/v1546288462/VOWAID/bg24.jpg"
          alt="meeting"
          class="responsive-img elevation-12 mb-3"
        >
        <h2 class="text-xs-center mt-3 twentyeight primary--text">VA Claims Process Assistance</h2>
        <v-divider class="mb-2"></v-divider>
        <p
          class="subheading secondary--text"
        >Our VOWAID TWS team is comprised of experienced Veterans who have dealt with serious issues with the VA personally. We understand how frustrating it can be to file a VA claim and get denied benefits. We also know how long that process can be. We are committed to helping you navigate through the VA, we help you understand the VA claims system, educate you on how to use e-benefits, my healthy vet and we will also do all the research for you and give you all the phone numbers you need i.e. VSOs, Patient Advocates as well as advocate for you if the system is failing to help you.</p>
      </v-flex>
      <v-flex xs12 md6 xl5 class="pa-5 fw">
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,q_70,w_800/v1546288508/VOWAID/w1.jpg"
          alt="woman on laptop"
          class="responsive-img elevation-12 mb-3"
        >
        <h2
          class="text-xs-center mt-3 twentyeight primary--text"
        >Domestic Violence Victim Recovery Assistance</h2>
        <v-divider class="mb-2"></v-divider>
        <p
          class="subheading secondary--text"
        >Our team is here to offer our Survivor Warriors with all the tools necessary to aid in rebuilding after surviving Intimate Partner Violence. We will connect you with local resources, community groups that are vetted through our case managers, and above all, a stigma and judgmental free environment to help the recovery process. Our seasoned and experienced team has been handpicked to be able to care, relate and understand what it takes to transition from being a Victim of Domestic Violence to becoming a Survivor Warrior that breaks the cycle of violence.</p>
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
    padding: 0 !important;
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

