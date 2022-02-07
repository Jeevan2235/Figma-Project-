<template>
  <div>
    <v-container>
      <v-card-title class="font-weight-black text-h4" style="font-size: 48px"
      >Latest News</v-card-title
    >
    </v-container>
    <v-row justify="center">
      <v-col v-for="child in childs" :key="child" cols="12" md="3">
        <v-card  class="mt-5">
          <v-img :src="child.img"></v-img>
          <v-card-title
            class="text-h5"
            >{{ child.title }}</v-card-title
          >
          <v-btn text color="#f31a1a" class="mb-8">{{ child.btn }}</v-btn>
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
        img: "2.png",
        title: "National Civil Society Conference 2021 Concludes",
        btn: "Read More",
      },
      {
        img: "4.png",
        title:
          "Narayana Murthy family contributes ₹10-crore towards Akshaya Patra’s COVID-19 Food Relief Service",
        btn: "Read More",
      },
      {
        img: "5.png",
        title: "73rd International Human Rights Day Observed",
        btn: "Read More",
      },
    ],
  }),
};
</script>

<style>
</style>