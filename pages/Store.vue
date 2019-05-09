<template>
  <v-container fluid>
    <v-layout row wrap justify-center align-center>
      <v-flex xs12 md6 lg4 xl3 class="text-xs-center">
        <v-hover>
          <v-card
            slot-scope="{ hover }"
            :class="`elevation-${hover ? 12 : 1}`"
            class="pa-4 ma-3 nuxtwhite"
          >
            <h4 class="display-1 primary--text">Donation</h4>
            <p class="subheading my-1">Use the options below to get your desired total.</p>
            <p
              class="body-1 mb-2"
            >Proceeds go to helping Veterans and their families in need. Donations can be used as a tax deduction.</p>
            <v-layout row wrap justify-center align-center>
              <v-flex>
                <v-btn
                  class="snipcart-add-item primary donations-btn"
                  large
                  round
                  data-item-id="0010D"
                  data-item-name="Donation"
                  data-item-price="10.00"
                  data-item-image="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,w_75/v1539460895/VOWAID/dollar-sign.png"
                  data-item-url="/products.json"
                  data-item-description="$10 Donation to VOWAID Foundation"
                >$10.00</v-btn>
              </v-flex>
              <v-flex>
                <v-btn
                  class="snipcart-add-item primary donations-btn"
                  large
                  round
                  data-item-id="0020D"
                  data-item-name="Donation"
                  data-item-price="20.00"
                  data-item-image="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,w_75/v1539460895/VOWAID/dollar-sign.png"
                  data-item-url="/products.json"
                  data-item-description="$25 Donation to VOWAID Foundation"
                >$20.00</v-btn>
              </v-flex>
              <v-flex>
                <v-btn
                  class="snipcart-add-item primary donations-btn"
                  large
                  round
                  data-item-id="0050D"
                  data-item-name="Donation"
                  data-item-price="50.00"
                  data-item-image="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,w_75/v1539460895/VOWAID/dollar-sign.png"
                  data-item-url="/products.json"
                  data-item-description="$50 Donation to VOWAID Foundation"
                >$50.00</v-btn>
              </v-flex>
              <v-flex>
                <v-btn
                  class="snipcart-add-item primary donations-btn"
                  large
                  round
                  data-item-id="0100D"
                  data-item-name="Donation"
                  data-item-price="100.00"
                  data-item-image="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,w_75/v1539460895/VOWAID/dollar-sign.png"
                  data-item-url="/products.json"
                  data-item-description="$100 Donation to VOWAID Foundation"
                >$100.00</v-btn>
              </v-flex>
              <v-flex xs12 class="hidden-sm-and-down">
                <img
                  src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,q_70,w_250/v1535429145/VOWAID/vowaid-logo-dark-shadow.png"
                  alt="logo"
                  class="responsive-img mt-4"
                >
              </v-flex>
            </v-layout>
          </v-card>
        </v-hover>
      </v-flex>

      <v-flex xs12 md6 lg4 xl3 class="text-xs-center">
        <v-hover>
          <v-card
            slot-scope="{ hover }"
            :class="`elevation-${hover ? 12 : 1}`"
            class="pa-4 ma-3 nuxtwhite"
          >
            <h4 class="headline primary--text">26XX SIGINT/EW Challenge Coin</h4>
            <h4 class="headline my-3">
              <small>$</small>
              25.00
            </h4>
            <img
              v-if="coinFlip"
              src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,q_50,h_230/v1535165336/VOWAID/26XX-coin-skull.png"
              alt="coin"
              class="responsive-img"
            >
            <img
              v-else
              src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,q_50,h_230/v1535165336/VOWAID/26XX-coin-squirrel.png"
              alt="coin"
              class="responsive-img"
            >
            <br>
            <br>
            <div style="width: 85%; text-align: right; margin-top: -50px;">
              <v-btn round small class="primary white--text" @click="flipCoin">flip</v-btn>
            </div>
            <p
              class="description-height"
              style="color: #333; font-weight: 400; padding-top: 15px;"
            >VOWAID and The Warrior Transition Club are proud to have paired with the 26XX Opportunities Community on this coin! Full color, 2", 26xx Skull and Secret Squirrel.</p>
            <v-btn
              class="snipcart-add-item primary white--text"
              large
              round
              data-item-id="2600C"
              data-item-name="26XX SIGINT/EW Challenge Coin"
              data-item-price="25.00"
              data-item-image="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,q_50,h_230/v1535165336/VOWAID/26XX-coin-squirrel.png"
              data-item-url="/products.json"
              data-item-description="Full color, 2&quot;, 26xx Skull and Secret Squirrel"
            >Add to Cart</v-btn>
          </v-card>
        </v-hover>
      </v-flex>
      <v-flex xs12 md6 lg4 xl3 class="text-xs-center">
        <v-hover>
          <v-card
            slot-scope="{ hover }"
            :class="`elevation-${hover ? 12 : 1}`"
            class="pa-4 ma-3 nuxtwhite"
          >
            <h4 class="display-1 primary--text">2621 Pin</h4>
            <h4 class="headline my-3">
              <small>$</small>
              10.00
            </h4>
            <img
              src="https://res.cloudinary.com/missionwebdev/image/upload/c_fill,f_auto,h_230,w_169/v1539732628/VOWAID/2621-pin.jpg"
              alt="2621 Pin"
              class="responsive-img"
            >
            <p
              class="description-height"
              style="color: #333; font-weight: 400; padding-top: 15px;"
            >VOWAID and The Warrior Transition Club are proud to have paired with the 26XX Opportunities Community on this pin! 1", 2621 pin.</p>
            <v-btn
              class="snipcart-add-item primary white--text"
              large
              round
              data-item-id="2621P"
              data-item-name="2621 Pin"
              data-item-price="10.00"
              data-item-image="https://res.cloudinary.com/missionwebdev/image/upload/c_fill,f_auto,h_230,w_169/v1539732628/VOWAID/2621-pin.jpg"
              data-item-url="/products.json"
              data-item-description="1&quot; 2621 Pin"
            >Add to Cart</v-btn>
          </v-card>
        </v-hover>
      </v-flex>
      <v-flex xs12 md6 lg4 xl3 class="text-xs-center">
        <v-hover>
          <v-card
            slot-scope="{ hover }"
            :class="`elevation-${hover ? 12 : 1}`"
            class="pa-4 ma-3 nuxtwhite"
          >
            <h4 class="display-1 primary--text">2641 Pin</h4>
            <h4 class="headline my-3">
              <small>$</small>
              10.00
            </h4>
            <img
              src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_230/v1539732628/VOWAID/2641-pin.jpg"
              alt="2641 Pin"
              class="responsive-img"
            >
            <p
              class="description-height"
              style="color: #333; font-weight: 400; padding-top: 15px;"
            >VOWAID and The Warrior Transition Club are proud to have paired with the 26XX Opportunities Community on this pin! 1", 2641 pin.</p>
            <v-btn
              class="snipcart-add-item primary white--text"
              large
              round
              data-item-id="2641P"
              data-item-name="2641 Pin"
              data-item-price="10.00"
              data-item-image="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_230/v1539732628/VOWAID/2641-pin.jpg"
              data-item-url="/products.json"
              data-item-description="1&quot; 2641 Pin"
            >Add to Cart</v-btn>
          </v-card>
        </v-hover>
      </v-flex>

      <v-flex xs12 md6 lg4 xl3 class="text-xs-center">
        <v-hover>
          <v-card
            slot-scope="{ hover }"
            :class="`elevation-${hover ? 12 : 1}`"
            class="pa-4 ma-3 nuxtwhite"
          >
            <h4 class="display-1 primary--text">2651 Pin</h4>
            <h4 class="headline my-3">
              <small>$</small>
              10.00
            </h4>
            <img
              src="https://res.cloudinary.com/missionwebdev/image/upload/c_fill,f_auto,h_230,w_169/v1539732628/VOWAID/2651-pin.jpg"
              alt="2651 Pin"
              class="responsive-img"
            >
            <p
              class="description-height"
              style="color: #333; font-weight: 400; padding-top: 15px;"
            >VOWAID and The Warrior Transition Club are proud to have paired with the 26XX Opportunities Community on this pin! 1", 2651 pin.</p>
            <v-btn
              class="snipcart-add-item primary white--text"
              large
              round
              data-item-id="2651P"
              data-item-name="2651 Pin"
              data-item-price="10.00"
              data-item-image="https://res.cloudinary.com/missionwebdev/image/upload/c_fill,f_auto,h_230,w_169/v1539732628/VOWAID/2651-pin.jpg"
              data-item-url="/products.json"
              data-item-description="1&quot; 2651 Pin"
            >Add to Cart</v-btn>
          </v-card>
        </v-hover>
      </v-flex>

      <v-flex xs12 md6 lg4 xl3 class="text-xs-center">
        <v-hover>
          <v-card
            slot-scope="{ hover }"
            :class="`elevation-${hover ? 12 : 1}`"
            class="pa-4 ma-3 nuxtwhite"
          >
            <h4 class="display-1 primary--text">26XX Decal</h4>
            <h4 class="headline my-3">
              <small>$</small>
              10.00
            </h4>
            <img
              src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_230/v1539732629/VOWAID/26XX-decal.jpg"
              alt="26XXDDecal"
              class="responsive-img"
            >
            <p
              class="description-height"
              style="color: #333; font-weight: 400; padding-top: 15px;"
            >VOWAID and The Warrior Transition Club are proud to have paired with the 26XX Opportunities Community on this decal! 3", 26XX Decal.</p>
            <v-btn
              class="snipcart-add-item primary white--text"
              large
              round
              data-item-id="26XXD"
              data-item-name="26XX Decal"
              data-item-price="10.00"
              data-item-image="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_230/v1539732629/VOWAID/26XX-decal.jpg"
              data-item-url="/products.json"
              data-item-description="3&quot; 26XX Decal"
            >Add to Cart</v-btn>
          </v-card>
        </v-hover>
      </v-flex>

      <v-flex xs12 md6 lg4 xl3 class="text-xs-center">
        <v-hover>
          <v-card
            slot-scope="{ hover }"
            :class="`elevation-${hover ? 12 : 1}`"
            class="pa-4 ma-3 nuxtwhite"
          >
            <h4 class="display-1 primary--text">2651 Decal</h4>
            <h4 class="headline my-3">
              <small>$</small>
              10.00
            </h4>
            <img
              src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_230/v1539732628/VOWAID/2651-decal.jpg"
              alt="2651 Decal"
              class="responsive-img"
            >
            <p
              class="description-height"
              style="color: #333; font-weight: 400; padding-top: 15px;"
            >VOWAID and The Warrior Transition Club are proud to have paired with the 26XX Opportunities Community on this decal! 3", 2651 Decal.</p>
            <v-btn
              class="snipcart-add-item primary white--text"
              large
              round
              data-item-id="2651D"
              data-item-name="2651 Decal"
              data-item-price="10.00"
              data-item-image="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_230/v1539732628/VOWAID/2651-decal.jpg"
              data-item-url="/products.json"
              data-item-description="3&quot; 2651 Decal"
            >Add to Cart</v-btn>
          </v-card>
        </v-hover>
      </v-flex>

      <v-flex xs12 md6 lg4 xl3 class="text-xs-center">
        <v-hover>
          <v-card
            slot-scope="{ hover }"
            :class="`elevation-${hover ? 12 : 1}`"
            class="pa-4 ma-3 nuxtwhite"
          >
            <h4 class="display-1 primary--text">2602 Decal</h4>
            <h4 class="headline my-3">
              <small>$</small>
              10.00
            </h4>
            <img
              src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_230/v1548123160/VOWAID/2602-decal.jpg"
              alt="2602 Decal"
              class="responsive-img"
            >
            <p
              class="description-height"
              style="color: #333; font-weight: 400; padding-top: 15px;"
            >VOWAID and The Warrior Transition Club are proud to have paired with the 26XX Opportunities Community on this decal! 3", 2602 Decal.</p>
            <v-btn
              class="snipcart-add-item primary white--text"
              large
              round
              data-item-id="2602D"
              data-item-name="2602 Decal"
              data-item-price="10.00"
              data-item-image="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_230/v1548123160/VOWAID/2602-decal.jpg"
              data-item-url="/products.json"
              data-item-description="3&quot; 2602 Decal"
            >Add to Cart</v-btn>
          </v-card>
        </v-hover>
      </v-flex>

      <v-flex xs12 md6 lg4 xl3 class="text-xs-center">
        <v-hover>
          <v-card
            slot-scope="{ hover }"
            :class="`elevation-${hover ? 12 : 1}`"
            class="pa-4 ma-3 nuxtwhite"
          >
            <h4 class="display-1 primary--text">2629 Decal</h4>
            <h4 class="headline my-3">
              <small>$</small>
              10.00
            </h4>
            <img
              src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_230/v1548123160/VOWAID/2629-decal.jpg"
              alt="2629 Decal"
              class="responsive-img"
            >
            <p
              class="description-height"
              style="color: #333; font-weight: 400; padding-top: 15px;"
            >VOWAID and The Warrior Transition Club are proud to have paired with the 26XX Opportunities Community on this decal! 3", 2629 Decal.</p>
            <v-btn
              class="snipcart-add-item primary white--text"
              large
              round
              data-item-id="2629D"
              data-item-name="2629 Decal"
              data-item-price="10.00"
              data-item-image="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_230/v1548123160/VOWAID/2629-decal.jpg"
              data-item-url="/products.json"
              data-item-description="3&quot; 2629 Decal"
            >Add to Cart</v-btn>
          </v-card>
        </v-hover>
      </v-flex>

      <v-flex xs12 md6 lg4 xl3 class="text-xs-center">
        <v-hover>
          <v-card
            slot-scope="{ hover }"
            :class="`elevation-${hover ? 12 : 1}`"
            class="pa-4 ma-3 nuxtwhite"
          >
            <h4 class="display-1 primary--text">267X Decal</h4>
            <h4 class="headline my-3">
              <small>$</small>
              10.00
            </h4>
            <img
              src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_230/v1548123159/VOWAID/267X-decal.jpg"
              alt="267X Decal"
              class="responsive-img"
            >
            <p
              class="description-height"
              style="color: #333; font-weight: 400; padding-top: 15px;"
            >VOWAID and The Warrior Transition Club are proud to have paired with the 26XX Opportunities Community on this decal! 3", 267X Decal.</p>
            <v-btn
              class="snipcart-add-item primary white--text"
              large
              round
              data-item-id="267XD"
              data-item-name="267X Decal"
              data-item-price="10.00"
              data-item-image="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_230/v1548123159/VOWAID/267X-decal.jpg"
              data-item-url="/products.json"
              data-item-description="3&quot; 267X Decal"
            >Add to Cart</v-btn>
          </v-card>
        </v-hover>
      </v-flex>

      <v-flex xs12 md6 lg4 xl3 class="text-xs-center">
        <v-hover>
          <v-card
            slot-scope="{ hover }"
            :class="`elevation-${hover ? 12 : 1}`"
            class="pa-4 ma-3 nuxtwhite"
          >
            <h4 class="display-1 primary--text">2691 Decal</h4>
            <h4 class="headline my-3">
              <small>$</small>
              10.00
            </h4>
            <img
              src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_230/v1548123159/VOWAID/2691-decal.jpg"
              alt="2691 Decal"
              class="responsive-img"
            >
            <p
              class="description-height"
              style="color: #333; font-weight: 400; padding-top: 15px;"
            >VOWAID and The Warrior Transition Club are proud to have paired with the 26XX Opportunities Community on this decal! 3", 2691 Decal.</p>
            <v-btn
              class="snipcart-add-item primary white--text"
              large
              round
              data-item-id="2691D"
              data-item-name="2691 Decal"
              data-item-price="10.00"
              data-item-image="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_230/v1548123159/VOWAID/2691-decal.jpg"
              data-item-url="/products.json"
              data-item-description="3&quot; 2691 Decal"
            >Add to Cart</v-btn>
          </v-card>
        </v-hover>
      </v-flex>

      <v-flex xs12 md6 lg4 xl3 class="text-xs-center">
        <v-hover>
          <v-card
            slot-scope="{ hover }"
            :class="`elevation-${hover ? 12 : 1}`"
            class="pa-4 ma-3 nuxtwhite"
          >
            <h4 class="display-1 primary--text">VOWAID Pin</h4>
            <h4 class="headline my-3">
              <small>$</small>
              10.00
            </h4>
            <img
              src="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_230,q_51/v1535440178/VOWAID/vowaid-pin.png"
              alt="pin"
              class="responsive-img"
            >
            <p
              class="description-height"
              style="color: #333; font-weight: 400; padding-top: 15px;"
            >1.65" VOWAID Foundation Pin.</p>
            <v-btn
              class="snipcart-add-item primary white--text"
              large
              round
              data-item-id="0001P"
              data-item-name="VOWAID Pin"
              data-item-price="20.00"
              data-item-image="https://res.cloudinary.com/missionwebdev/image/upload/c_scale,f_auto,h_300,q_51/v1535440178/VOWAID/vowaid-pin.png"
              data-item-url="/products.json"
              data-item-description="1&quot; White VOWAID Pin"
            >Add to Cart</v-btn>
          </v-card>
        </v-hover>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
let coinFlip = true;

// Snipcart.execute("config", "show_continue_shopping", true);

export default {
  data() {
    return {
      coinFlip: true
    };
  },
  methods: {
    flipCoin() {
      this.coinFlip = !this.coinFlip;
    }
  }
};
</script>

<style lang="scss" scoped>
@media screen and (min-width: 960px) {
  .description-height {
    height: 80px;
  }
  .v-card {
    height: 570px;
  }
}
.donations-btn {
  width: 140px;
}
</style>
