<template>
  <div class="bg-color">
    <v-container fluid>
      <v-card class="" tile elevation="0" color="transparent">
        <v-row>
          <v-col md="6">
            <v-card-title class="font-weight-black text-h4"
              >Upcoming Events</v-card-title
            >
            <v-card
              v-for="card in cards"
              :key="card"
              tile
              color="#e5e5e5"
              elevation="0"
            >
              <v-row>
                <v-col md="4">
                  <v-img :src="card.img" class="mt-5"></v-img>
                </v-col>
                <v-col md="8">
                  <v-card-title style="font-size: 26px; font-weight: 600">{{
                    card.title
                  }}</v-card-title>
                  <v-card-text>{{ card.date }}</v-card-text>
                  <v-card-text>{{ card.text }}</v-card-text>
                  <v-btn text color="#f31a1a">{{ card.btn }}</v-btn>
                </v-col>
              </v-row>
            </v-card>
          </v-col>
          <v-col md="6">
            <v-card-title class="font-weight-black text-h4"
              >Featured Cause</v-card-title
            >
            <v-card
              color="#0c2059"
              v-for="kid in kids"
              :key="kid"
              class="mt-16"
              tile
            >
              <v-row>
                <v-col md="6">
                  <v-img :src="kid.img" class="ma-5"></v-img>
                </v-col>
                <v-col md="6">
                  <v-card-title class="white--text" style="font-size: 26px">{{
                    kid.title
                  }}</v-card-title>
                  <v-card-text class="white--text">{{ kid.date }}</v-card-text>
                  <v-card-text
                    class="white--text"
                    style="font-size: 16px; padding-right: 60px"
                    >{{ kid.text }}</v-card-text
                  >
                  <v-btn
                    color="#f94f19"
                    rounded
                    class="white--text ml-3 mt-12"
                    >{{ kid.btn }}</v-btn
                  >
                </v-col>
                <v-card-text class="pt-0">
                  <v-slider
                    v-model="value"
                    class="ma-3"
                    :rules="rules"
                    step="10"
                    thumb-label="always"
                    color="#f94f19"
                    ticks
                  ></v-slider>
                  <v-row>
                    <v-col>
                      <v-card-text class="white--text"
                        >Raised : Rs 1,60,000</v-card-text
                      >
                    </v-col>
                    <v-col md="4">
                      <v-card-text class="white--text"
                        >Raised : Rs 1,60,000</v-card-text
                      >
                    </v-col>
                  </v-row>
                </v-card-text>
              </v-row>
            </v-card>
          </v-col>
        </v-row>
      </v-card>
    </v-container>
  </div>
</template>

<script>
export default {
  data: () => ({
    cards: [
      {
        img: "19.png",
        title: "Fundraiser for Kids ",
        date: "8th Aug 2018     |    Kathmandu",
        text: " Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris.",
        btn: "Read More",
      },
      {
        img: "17.png",
        title: "Bring water to the childrens",
        date: "8th Aug 2018     |    Kathmandu",
        text: " Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris.",
        btn: "Read More",
      },
      {
        img: "17.png",
        title: "Bring water to the childrens",
        date: "8th Aug 2018     |    Kathmandu",
        text: " Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris.",
        btn: "Read More",
      },
    ],

    kids: [
      {
        img: "18.png",
        title: "Fundraiser for Kids ",
        date: "8th Aug 2018     |    Kathmandu",
        text: " Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris.",
        btn: "Donate Now",
      },
    ],
  }),
};
</script>

<style scoped>
.bg-color {
  background: #e5e5e5;
}
</style>