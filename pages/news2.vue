<template>
  <v-container class="mt-16">
    <h1>National Civil Society Conference 2021 Concludes</h1>
    <v-row>
      <v-col class="mt-5" md="7">
        <v-card v-for="link in links" :key="link" tile  elevation="0">
          <v-img :src="link.img" class="mt-10"></v-img>
          <p style="font-size: 18px; text-align: justify">{{ link.text }}</p>
          <v-img :src="link.img2" ></v-img>
          <p style="font-size: 18px; text-align: justify; line-height: 25px">
            {{ link.text2 }}
          </p>
           <div>
            <v-row class="mt-5 mb-8">
              <v-col cols="12" md="4">
                <v-btn class="white--text" color="#163fb2" rounded height="4em" small>
                  <v-icon class="mr-2"  color="white"> mdi-facebook </v-icon>
                  Share on facebook
                </v-btn>
              </v-col>
              <v-col cols="12" md="4">
                <v-btn class="white--text" color="#15aabe" rounded height="4em" small
                  ><v-icon class="mr-2"  color="white"> mdi-twitter </v-icon> Share on
                  twitter</v-btn
                >
              </v-col>
              <v-col>
                <v-btn class="white--text" color="#f31a1a" height="4em" rounded small
                  ><v-icon class="mr-2"  color="white"> mdi-instagram </v-icon> Share on
                  instagram</v-btn
                >
              </v-col>
            </v-row>
          </div>

          <div class="text-center">
            <v-row>
              <v-col cols="12" md="4">
                <v-card-text>Comments:</v-card-text>
              </v-col>
              <v-col cols="12" md="6">
                <v-text-field label="Email...." outlined></v-text-field>
                <v-textarea label="Message..." outlined></v-textarea>
              </v-col>
            </v-row>
            <v-btn
              class="mt-3 ml-12 white--text"
              color="#f94f19"
              rounded
              elevation="0"
              height="2.5em"
              width="9em"
              >Submit</v-btn
            >
          </div>
        </v-card>
      </v-col>
      <v-col md="5" class="mt-14">
        <v-card
          color="#e5e5e5"
          class="ma-2"
          v-for="thing in things"
          :key="thing"
        >
          <v-card-title>{{ thing.title }}</v-card-title>
          <v-card-text style="color: #000000; font-weight: 600">{{
            thing.title2
          }}</v-card-text>
          <v-card-text style="text-align: justify;">{{ thing.text }}</v-card-text>
          <v-btn text color="#f31a1a" rounded elevation="0" width="9em">{{
            thing.btn
          }}</v-btn>
        </v-card>
      </v-col>
    </v-row>

    
      <p class="font-weight-black text-h4 mt-16">Other News</p>
      <latest-2 />
    
  </v-container>
</template>

<script>
import latest2 from "../components/latest2.vue";
export default {
  components: { latest2 },
  data: () => ({
    buttons: [
      {
        icon: "mdi-facebook",
        text: "Share on facebook",
      },
    ],
    links: [
      {
        img: "2.png",
        text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris. Lorem ipsum dolor sit amet, consectetur. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris quis aliquam. Integer accumsan sodales odio, id tempus velit ullamc. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris. Lorem ipsum dolor sit amet, consectetur. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris. Lorem ipsum dolor sit amet, consectetur. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris quis aliquam. Integer accumsan sodales odio, id tempus velit ullamc. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris. Lorem ipsum dolor sit amet, consectetur. ",
        img2: "3.png",
        text2:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris. Lorem ipsum dolor sit amet, consectetur. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris quis aliquam. Integer accumsan sodales odio, id tempus velit ullamc. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris. Lorem ipsum dolor sit amet, consectetur. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris. Lorem ipsum dolor sit amet, consectetur. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris quis aliquam. Integer accumsan sodales odio, id tempus velit ullamc. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris. Lorem ipsum dolor sit amet, consectetur.  ",
      },
    ],
  

    things: [
      {
        title: "Related Stories",
        title2:
          "Narayana Murthy family contributes ₹10-crore towards Akshaya Patra’s COVID-19 Food Relief Service",
        text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris. Lorem ipsum dolor sit amet, consectetur. ",
        btn: "Read More",
      },
      {
        title: "Related Stories",
        title2:
          "Narayana Murthy family contributes ₹10-crore towards Akshaya Patra’s COVID-19 Food Relief Service",
        text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris. Lorem ipsum dolor sit amet, consectetur. ",
        btn: "Read More",
      },
      {
        title: "Related Stories",
        title2:
          "Narayana Murthy family contributes ₹10-crore towards Akshaya Patra’s COVID-19 Food Relief Service",
        text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris. Lorem ipsum dolor sit amet, consectetur. ",
        btn: "Read More",
      },
    ],
  }),
};
</script>

<style>
</style>