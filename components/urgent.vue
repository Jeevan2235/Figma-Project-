<template>
  <div>
    <v-container>
      <v-card-title class="font-weight-black text-h4">Urgent Causes</v-card-title>
    </v-container>
    <v-row justify="center">
      <v-col cols="12" md="3" v-for="child in childs" :key="child">
        <v-card class="mt-5">
          <v-img :src="child.img"></v-img>
          <v-card-title class="font-weight-black text-h6">{{
            child.title
          }}</v-card-title>
          <v-card-text>{{ child.text }}</v-card-text>
          <v-card-text
            class="mb-8"
            style="
              color: #000000;
              font-size: 16px;
              font-weight: 400;
            "
            >{{ child.text2 }}</v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  data: () => ({
    childs: [
      {
        img: "8.png",
        title: "Bring water to the childrens",
        text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris.",
        text2: " Rs 5,00,000 Needed donation",
      },
      {
        img: "11.png",
        title: "Education for all",
        text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris.",
        text2: " Rs 5,00,000 Needed donation",
      },
      {
        img: "10.png",
        title: "Proper elderly care",
        text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris.",
        text2: " Rs 5,00,000 Needed donation",
      },
    ],
  }),
};
</script>

<style>
</style>