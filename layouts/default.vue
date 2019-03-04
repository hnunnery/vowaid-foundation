<template>
  <v-app class="app">
    <v-toolbar app scroll-off-screen>
      <v-flex class="text-xs-center">
        <nuxt-link to="/">
          <img
            src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,w_160/v1534824485/VOWAID/navbar-logo.png"
            alt="logo"
            id="navbar-logo"
            class="pt-2"
          >
        </nuxt-link>
      </v-flex>
      <!-- NAVBAR FOR MEDIUM AND UP SCREEN SIZES -->
      <v-toolbar-items class="hidden-md-and-down">
        <v-btn flat to="/">
          <v-icon class="primary--text navbar-icons">fas fa-home</v-icon>&nbsp;
          <span class="nav-text primary--text">Home</span>
        </v-btn>
        <v-btn flat to="/services">
          <v-icon class="primary--text navbar-icons">fas fa-hands-helping</v-icon>&nbsp;
          <span class="nav-text primary--text">Services</span>
        </v-btn>
        <v-btn flat to="/store">
          <v-icon class="primary--text navbar-icons">fas fa-store</v-icon>&nbsp;
          <span class="nav-text primary--text">Store</span>
        </v-btn>
        <v-btn flat to="/sponsors">
          <v-icon class="primary--text navbar-icons">fas fa-address-card</v-icon>&nbsp;
          <span class="nav-text primary--text">Sponsors</span>
        </v-btn>
        <v-btn flat to="/events">
          <v-icon class="primary--text navbar-icons">fas fa-calendar-alt</v-icon>&nbsp;
          <span class="nav-text primary--text">Events</span>
        </v-btn>
        <v-btn flat to="/about">
          <v-icon class="primary--text navbar-icons">fas fa-user-circle</v-icon>&nbsp;
          <span class="nav-text primary--text">About</span>
        </v-btn>
        <!-- <v-btn flat to="/blog">
          <v-icon class="primary--text navbar-icons">fas fa-blog</v-icon>&nbsp;
          <span class="nav-text primary--text">Blog</span>
        </v-btn>-->
        <v-btn flat to="/contact">
          <v-icon class="primary--text navbar-icons">fas fa-envelope</v-icon>&nbsp;
          <span class="nav-text primary--text">Contact</span>
        </v-btn>
        <v-btn flat class="snipcart-checkout">
          <span class="snipcart-summary snipcart-summary-empty">
            <v-icon class="primary--text navbar-icons">fas fa-shopping-cart</v-icon>
            <span class="snipcart-total-price nav-text primary--text"></span>
          </span>
        </v-btn>
      </v-toolbar-items>
      <!-- NAVBAR FOR SMALL AND EXTRA SMALL SCREEN SIZES -->
      <v-btn icon @click.stop="rightDrawer = !rightDrawer" class="hidden-lg-and-up">
        <v-icon class="darkgrey--text">fas fa-bars</v-icon>
      </v-btn>
    </v-toolbar>

    <v-navigation-drawer
      clipped
      temporary
      width="180"
      :right="right"
      v-model="rightDrawer"
      class="hidden-lg-and-up"
      fixed
      app
    >
      <v-list>
        <img
          src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,q_100,w_130/v1535429145/VOWAID/vowaid-logo-dark-shadow.png"
          alt="logo"
          class="responsive-img ml-4 my-3 text-xs-left"
        >
        <v-list-tile to="/" class="sidenav-element">
          <v-list-tile-action>
            <v-icon class="primary--text text-xs-center">fas fa-home</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title class="primary--text nav-font-size font-weight-medium">Home</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile to="/services" class="sidenav-element">
          <v-list-tile-action>
            <v-icon class="primary--text text-xs-center">fas fa-hands-helping</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title class="primary--text nav-font-size font-weight-medium">Services</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile to="/store" class="sidenav-element">
          <v-list-tile-action>
            <v-icon class="primary--text text-xs-center">fas fa-store</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title class="primary--text nav-font-size font-weight-medium">Store</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile to="/sponsors" class="sidenav-element">
          <v-list-tile-action>
            <v-icon class="primary--text text-xs-center">fas fa-address-card</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title class="primary--text nav-font-size font-weight-medium">Sponsors</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile to="/events" class="sidenav-element">
          <v-list-tile-action>
            <v-icon class="primary--text text-xs-center">fas fa-calendar-alt</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title class="primary--text nav-font-size font-weight-medium">Events</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile to="/about" class="sidenav-element">
          <v-list-tile-action>
            <v-icon class="primary--text text-xs-center">fas fa-user-circle</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title class="primary--text nav-font-size font-weight-medium">About</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <!-- <v-list-tile to="/blog" class="sidenav-element">
          <v-list-tile-action>
            <v-icon class="primary--text text-xs-center">fas fa-blog</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title class="primary--text nav-font-size font-weight-medium">Blog</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>-->
        <v-list-tile to="/contact" class="bottom-sidenav-element sidenav-element">
          <v-list-tile-action>
            <v-icon class="primary--text text-xs-center">fas fa-envelope</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title class="primary--text nav-font-size font-weight-medium">Contact</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile class="snipcart-summary snipcart-summary-empty snipcart-checkout">
          <v-list-tile-action class="nav-link">
            <v-icon class="primary--text text-xs-center">fas fa-shopping-cart</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title class="primary--text nav-font-size font-weight-medium">
              <span class="snipcart-total-price"></span>
            </v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>

    <v-content>
      <router-view/>
    </v-content>

    <v-footer height="auto" class="page-footer">
      <v-card flat tile color="#111" class="flex">
        <v-layout row wrap justify-center align-center class="mt-2 mb-3">
          <v-flex xs12 class="text-xs-center mb-2">
            <v-btn class="mx-3" dark icon>
              <a href="https://www.facebook.com/vowaid" target="_blank">
                <v-icon size="32px">fab fa-facebook</v-icon>
              </a>
            </v-btn>
            <v-btn class="mx-3" dark icon>
              <a href="https://twitter.com/vow_aid" target="_blank">
                <v-icon size="32px">fab fa-twitter</v-icon>
              </a>
            </v-btn>
            <v-btn class="mx-3" dark icon>
              <a href="https://www.instagram.com/vow_aid" target="_blank">
                <v-icon size="32px">fab fa-instagram</v-icon>
              </a>
            </v-btn>
          </v-flex>
          <v-flex xs12 class="text-xs-center">
            <v-layout row wrap>
              <v-flex xs12 md6>
                <p class="white--text">
                  Created by
                  <a href="https://www.codehunter.io" target="_blank">
                    <span class="b-align">code</span>
                    <span class="text--white font-weight-bold">Hunter</span>
                  </a> Web Design and Development
                </p>
              </v-flex>
              <v-flex xs12 md6>
                <p class="white--text">© 2019 Veterans of War Aid Foundation</p>
              </v-flex>
            </v-layout>
          </v-flex>
        </v-layout>
      </v-card>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: "app",
  data() {
    return {
      clipped: false,
      drawer: true,
      fixed: false,
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: "Vuetify.js"
    };
  }
};
</script>

<style lang="scss" scoped>
// NAVBAR - size logo
#navbar-logo {
  max-height: 45px;
  align-items: center;
  margin-left: 36px;
  padding-top: 2px;
  @media screen and (min-width: 1500px) {
    display: block;
    margin-left: 24px;
  }
}
.navbar-icons {
  font-size: 1.4em;
}
.nav-font-size {
  font-size: 1.3em;
}
.nav-text {
  padding-left: 5px;
  font-size: 1.4em;
  text-transform: capitalize;
}

// NAVBAR - raising fontawesome5 icons
.fa,
.fab,
.fal,
.far,
.fas {
  @media only screen and (max-width: 958px) {
    vertical-align: text-top;
  }
}
/* STYLE NAVIGATION DRAWER */
.v-list {
  padding: 0 !important;
  .fa-home {
    margin-left: 1px;
  }
  .fa-calendar-alt {
    margin-left: 3px;
  }
  .fa-user-circle,
  .fa-blog,
  .fa-envelope {
    margin-left: 2px;
  }
}

// FOOTER - bottom aligns text in codeHunter
.b-align {
  vertical-align: bottom;
  line-height: 18px;
  color: #22aa00;
  font-size: 0.85em;
  margin-right: -2px;
}
.page-footer {
  /* border-top: 1px solid #2a2968; */
  p {
    margin: 3px auto;
  }
}
</style>