<template>
  <v-app>
    <v-card tile color="#0c2059" class="px-16">
        <v-row justify="center">
          <v-col cols="12" md="6" >
            <div class="d-sm-flex align-center justify-space-between">
              <div class="py-2">
                <v-icon small color="white"> mdi-map-marker </v-icon>
                <span class="white--text">Gyaneshwor, Kathmandu</span>
              </div>
              <div class="py-2">
                <v-icon small color="white"> mdi-phone </v-icon>
                <span class="white--text">01-5900919</span>
              </div>
              <div class="py-2">
                <v-icon small color="white"> mdi-email </v-icon>
                <span class="white--text">info@hospital.com</span>
              </div>
            </div>
          </v-col>
          <v-col md="4"></v-col>
          <v-col cols="12" md="2">
              <v-icon size="30" class="" color="white"> mdi-facebook </v-icon>
              <v-icon size="30" class="ml-3" color="white">mdi-twitter</v-icon>
              <v-icon size="30" class="ml-3" color="white">mdi-linkedin</v-icon>
              <v-icon size="30" class="ml-3" color="white">mdi-youtube</v-icon>
          </v-col>
      </v-row>
    </v-card>
    <top />
    <v-main>
      <Nuxt />
    </v-main>
    <v-footer color="#0c2059" >
      <v-card flat tile color="#0c2059" class="white--text text-center">
        <v-row class="mt-10 ma-10">
          <v-col md="3">
            <v-card-text
              class="mt-10"
              style="font-size: 18px; text-align: justify"
              >Lorem ipsum dolor sit amet, con sectetur adipiscing elit. Mauris
              temp us vestib ulum mauris.Lorem ipsum dolor sit amet, consectetur
              adipiscing elit. Mauris tempus vestib ulum mauris.Lorem ipsum
              dolo..........</v-card-text
            >
            <v-btn
              v-for="icon in icons"
              :key="icon"
              class="mx-4 white--text"
              icon
            >
              <v-icon size="24px">
                {{ icon }}
              </v-icon>
            </v-btn>
          </v-col>

          <v-col md="2" style="font-size: 18px">
            <div style="text-align: justify">
              <h3>Useful Links</h3>
              <p class="mt-8">Home</p>
              <p>About Us</p>
              <p>Causes</p>
              <p>Gallery</p>
              <p>News</p>
              <p>Contact</p>
            </div>
          </v-col>

          <v-col md="4" style="font-size: 18px">
            <div style="text-align: justify">
              <h3>Latest News</h3>
              <p class="mt-8">
                National Civil Society
                <br />
                Conference 2021 Concludes
              </p>
              <p>
                73rd International Human <br />
                Rights Day Observed
              </p>
              <p>We love to help people</p>
            </div>
          </v-col>
          <v-col cols="12" md="3" style="font-size: 18px">
            <div style="text-align: justify">
              <h3>Contact</h3>

              <v-row class="mt-5">
                <v-col cols="12" md="12">
                  <v-icon color="white"> mdi-phone </v-icon>
                  +977-9876548976
                </v-col>
              </v-row>
              <v-row>
                <v-col cols="12" md="12">
                  <v-icon color="white"> mdi-email </v-icon>
                  asd@gmail.com
                </v-col>
              </v-row>
              <v-row>
                <v-col cols="12" md="12">
                  <v-icon color="white"> mdi-map-marker </v-icon>
                  Gyaneshwor, Kathmandu
                </v-col>
              </v-row>
            </div>

            <v-row class="mt-5">
              <v-text-field label="Your email..." class="" solo> </v-text-field>
            </v-row>
          </v-col>
        </v-row>
      </v-card>
    </v-footer>
    <v-card class="white--text" tile color="#000000">
      <p class="ma-5 text-center">
        Copyright ©2021 All rights reserved | This design is made by Code
        Asterisk Pvt. Ltd
      </p>
    </v-card>
  </v-app>
</template>

<script>
import Top from "../components/top.vue";

export default {
  components: { Top },

  data: () => ({
    icons: ["mdi-facebook", "mdi-twitter", "mdi-linkedin", "mdi-instagram"],
    selectedItem: 1,
    items: [
      { text: "+977-9876548976", icon: "mdi-phone" },
      { text: "asd@gmail.com", icon: "mdi-email" },
      { text: "Gyaneshwor, Kathmandu", icon: "mdi-map-marker" },
    ],
  }),
};
</script>

<style>
</style>