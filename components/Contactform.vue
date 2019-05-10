<template>
  <div class="page-wrapper">
    <v-container class="py-3">
      <v-layout wrap justify-space-around>
        <v-flex xs12 sm9 md6 xl4>
          <v-card class="elevation-12 my-4 nuxtwhite">
            <v-card-text>
              <form
                name="contact"
                method="POST"
                data-netlify="true"
                data-netlify-honeypot="bot-field"
                class="pa-4"
              >
                <!-- NETLIFY FORM NAME -->
                <input type="hidden" name="form-name" value="contact">
                <!-- NETLIFY BOT FIELD -->
                <input type="text" name="bot-field" class="hidden">
                <h2 class="primary--text text-xs-center display-3">Contact Us</h2>
                <input type="text" name="name" placeholder="Name" required class="my-4">
                <input type="email" name="email" placeholder="Email" required class="my-4">
                <input type="phone" name="phone" placeholder="Phone" required class="my-4">
                <input type="address" name="address" placeholder="Address" required class="my-4">
                <input
                  type="branch_of_service"
                  name="branch_of_service"
                  placeholder="Branch of Service"
                  required
                  class="my-4"
                >
                <input type="rank" name="rank" placeholder="Rank" required class="my-4">
                <input
                  type="discharge_type"
                  name="discharge_type"
                  placeholder="Type of Discharge"
                  required
                  class="my-4"
                >
                <textarea name="message" placeholder="Message" rows="4" required class="my-4"></textarea>
                <div class="text-xs-center">
                  <v-btn large round type="submit" class="primary mt-4">Submit</v-btn>
                </div>
              </form>
            </v-card-text>
          </v-card>
        </v-flex>
        <v-flex xs12 md6 lg5 xl4>
          <img
            src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,q_100,w_705/v1535429145/VOWAID/vowaid-logo-dark-shadow.png"
            alt="logo"
            class="responsive-img mt-5"
            data-aos="fade-left"
            data-aos-delay="200"
            data-aos-duration="1000"
          >
          <div class="my-5">
            <div class="text-xs-left">
              <a href="mailto:contact@vowaidfoundation.org">
                <v-layout class="pb-4">
                  <v-flex xs3 class="text-xs-center">
                    <v-icon size="45px" class="primary--text">fas fa-envelope</v-icon>
                  </v-flex>
                  <v-flex xs9>
                    <h4 class="secondary--text display-1">
                      Send
                      <span class="hide-on-mobile">us</span> an email
                    </h4>
                    <p class="secondary--text subheading">contact@vowaidfoundation.org</p>
                  </v-flex>
                </v-layout>
              </a>
            </div>
            <div class="col s12 text-xs-left">
              <a href="tel:781-486-3408">
                <v-layout class="pb-4">
                  <v-flex xs3 class="text-xs-center">
                    <v-icon size="45px" class="primary--text">fas fa-mobile-alt</v-icon>
                  </v-flex>
                  <v-flex xs9>
                    <h4 class="secondary--text display-1">Give us a ring</h4>
                    <p class="secondary--text subheading">(781) 486-3408</p>
                  </v-flex>
                </v-layout>
              </a>
            </div>
            <div class="col s12 text-xs-left">
              <v-layout class="pb-4">
                <v-flex xs3 class="text-xs-center">
                  <v-icon size="45px" class="primary--text">fas fa-map-marked-alt</v-icon>
                </v-flex>
                <v-flex xs9>
                  <h4 class="secondary--text display-1">
                    <span class="hide-on-mobile">Mailing</span> Address
                  </h4>
                  <p class="secondary--text subheading">
                    2307 S. Rural Road
                    <br>Tempe, Arizona 85282
                  </p>
                </v-flex>
              </v-layout>
            </div>
          </div>
        </v-flex>
      </v-layout>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "contact-form"
};
</script>

<style lang="scss" scoped>
.page-wrapper {
  min-height: 100vh;
}

@media screen and (max-width: 399px) {
  .container {
    padding: 5px !important;
  }
}

input,
textarea,
select,
.sixteen {
  font-size: 16px;
}

input,
textarea {
  width: 100%;
  display: block;
  border: none;
  padding: 30px 0 0 0;
  border-bottom: solid 1px var(--orange);
  transition: all 0.3s cubic-bezier(0.64, 0.09, 0.08, 1);
  &:focus,
  &:valid {
    box-shadow: none;
    outline: none;
    background-position: 0 0;
    &::-webkit-input-placeholder {
      color: var(--orange);
      font-size: 11px;
      transform: translateY(-20px);
      visibility: visible !important;
    }
  }
}
</style>

<style lang="scss" scoped>
/* CSS for Select Component */
.custom-select select {
  width: 100%;
  height: 100%;
  background: none;
  border: none;
  -webkit-appearance: none;
  padding: 0 50px 0 20px;
  cursor: pointer;
  text-indent: 5px;
}

.custom-select .select {
  position: relative;
  background: #fff;
  border: 1px solid var(--orange);
  height: 50px;
  cursor: pointer;
}

.custom-select .select:focus {
  outline: none;
}

.custom-select .select:before {
  content: "";
  background: var(--orange);
  position: absolute;
  top: 0;
  bottom: 0;
  right: 0;
  width: 40px;
  pointer-events: none;
}

.custom-select .select:after {
  content: "";
  width: 0;
  height: 0;
  border-style: solid;
  border-width: 10px 7px 0;
  border-color: #fff transparent transparent transparent;
  position: absolute;
  top: 50%;
  right: 12px;
  transform: translateY(-50%);
}

.custom-select .select::-ms-expand {
  display: none;
}
</style>