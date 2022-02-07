<template>
  <div class="bg" >
    <v-container>
      <v-card-title class="font-weight-black text-h5"
        >Our Team Members
      </v-card-title>
      <v-row justify="center">
        <v-col v-for="child in childs" :key="child" cols="12" md="3">
          <v-card class="mt-16">
            <v-img :src="child.img"></v-img>

            <v-card-text
              style="color: #0c2059; font-size: 16px; font-weight: bold"
              >{{ child.text }}</v-card-text
            >
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data: () => ({
    childs: [
      {
        img: "33.png",
        text: "Miss Susmita Khatri",
      },
      {
        img: "29.png",
        text: "Mr Bishnu Thapa",
      },
      {
        img: "31.png",
        text: "Miss Asmita Sapkota",
      },
      {
        img: "34.png",
        text: "Mr Krishna Subedi",
      },
      {
        img: "28.png",
        text: "Mr Suman Basnet",
      },
      {
        img: "30.png",
        text: "Miss Samana Shrestha",
      },
      {
        img: "32.png",
        text: "Mr Aryan Baniya",
      },
      {
        img: "27.png",
        text: "Mr Sanjaya Khanal",
      },
    ],
  }),
};
</script>

<style scoped>
.bg {
  background-color: #e5e5e5;
}
</style>