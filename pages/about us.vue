<template>
  <div >
    <v-img src="26.png">
      <v-row justify="center">
        <h1
          class="white--text font-weight-black text-h2"
          style="font-size: 72px; margin-top: 120px"
        >
          About Us
        </h1>
      </v-row>
    </v-img>
    <v-container>
      <v-card v-for="link in links" :key="link" class="mt-16" elevation="0">
        <v-row>
          <v-col cols="12" md="6">
            <v-card-title class="font-weight-black text-h4">{{
              link.title
            }}</v-card-title>
            <v-card-text
              class="mt-5"
              style="text-align: justify; line-height: 36px; font-size: 24px"
              >{{ link.text }}</v-card-text
            >
          </v-col>
          <v-col cols="12" md="6">
            <v-img :src="link.img"></v-img>
          </v-col>
        </v-row>
      </v-card>
      </v-container>
      <teammember />
    
  </div>
</template>

<script>
import teammember from "../components/teammember.vue";
export default {
  components: { teammember },
  data: () => ({
    links: [
      {
        img: "25.png",
        title: "About Our NGO",
        text: "Lorem ipsum dolor sit amet, con sectetur adipiscing elit. Mauris temp us vestib ulum mauris.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris.Lorem ipsum dolo.Lorem ipsum dolor sit amet, con sectetur adipiscing elit. Mauris temp us vestib ulum mauris.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris.Lorem ipsum dolo..........",
      },
    ],
  }),
};
</script>

<style>
</style>