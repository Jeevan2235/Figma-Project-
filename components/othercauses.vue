<template>
  <v-container>
    <v-card-title class="font-weight-black text-h4">Other Causes</v-card-title>
    <v-row>
      <v-col v-for="link in links" :key="link" cols="12" md="4">
        <v-card
          class="d-flex flex-column justify-end"
          min-height="400"
          elevation="0"
          width="100%"
          :img="link.img"
        >
          <v-card class="ml-4" width="60%" tile color="#f94f19">
            <p class="white--text" style="font-size: 48px">
              {{ link.text }}
            </p>
          </v-card>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    links: [
      {
        img: "14.png",
        text: "Children needs food.",
      },
      {
        img: "15.png",
        text: "Fighting malnutrition in kids.",
      },
      {
        img: "16.png",
        text: "Help senior citizens.",
      },
    ],
  }),
};
</script>

<style>
</style>