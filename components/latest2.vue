<template>
 <v-container >
    <v-row justify="center">
   <v-col cols="12" md="4" v-for="child in childs" :key="child">
      <v-card  >
      <v-img :src="child.img"></v-img>
      <v-card-title
       class=" text-h5"
        >{{ child.title }}</v-card-title
      >
      <v-btn text color="#f31a1a" class="mb-8">{{ child.btn }}</v-btn>
    </v-card>
   </v-col>
  </v-row>
 </v-container>
</template>

<script>
export default {
  data: () => ({
    childs: [
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
      {
        img: "5.png",
        title: "73rd International Human Rights Day Observed",
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