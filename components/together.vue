<template>
  <v-container fluid>
    <v-card elevation="0" tile>
      <v-row>
        <v-col v-for="thing in things" :key="thing" cols="12" md="6">
          <v-card-title class="mt-10 font-weight-black text-h2">{{
            thing.title
          }}</v-card-title>
          <v-card-title class="font-weight-black text-h2">{{
            thing.title2
          }}</v-card-title>
          <v-card-title class="font-weight-black text-h2">{{
            thing.title3
          }}</v-card-title>
          <v-card-text
            class="mt-15"
            style="font-size: 26px; line-height: 40px; text-align: justify"
            >{{ thing.text }}</v-card-text
          >
          <v-btn
            class="mt-5 ml-4 white--text"
            color="#f94f19"
            rounded
            elevation="0"
            height="2.5em"
            width="9em"
          >
            Read More</v-btn
          >
        </v-col>

        <v-col cols="12" md="5">
          <v-row>
            <v-col cols="12" v-for="image in images" :key="image" md="6">
              <v-img :src="image.img"></v-img>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-card>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    things: [
      {
        title: "Together We are",
        title2: "Strengthening ",
        title3: " Humanity",
        text: "Lorem ipsum dolor sit amet, con sectetur adipiscing elit. Mauris temp us vestib ulum mauris.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris.Lorem ipsum dolo.",
      },
    ],

    images: [
      {
        img: "21.png",
      },
      {
        img: "22.png",
      },
      {
        img: "23.png",
      },
      {
        img: "24.png",
      },
    ],
  }),
};
</script>

<style>
</style>