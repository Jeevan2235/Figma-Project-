<template>
  <div>
    <v-img src="12.png"> </v-img>

    <v-container>
      <v-card color="#e5e5e5" v-for="link in links" :key="link" class="mt-12">
        <v-row justify="center">
          <v-col cols="12" md="8">
            <v-card-title style="font-size: 30px">{{
              link.title
            }}</v-card-title>
            <v-card-text
              style="line-height: 30px; text-align: justify; font-size: 18px"
              >{{ link.text }}</v-card-text
            >
            <v-btn color="#f31a1a" text>{{ link.btn }}</v-btn>
          </v-col>
          <v-col cols="12" md="4">
            <v-img :src="link.img"></v-img>
          </v-col>
        </v-row>
      </v-card>
    </v-container>
  </div>
</template>

<script>
export default {
  data: () => ({
    links: [
      {
        title: "National Civil Society Conference 2021 Concludes",
        text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris. Lorem ipsum dolor sit amet, consectetur. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris quis aliquam. Integer accumsan sodales odio, id tempus velit ullamc.",
        btn: "Read more",
        img: "2.png",
      },
      {
        title:
          "Narayana Murthy family contributes ₹10-crore towards Akshaya Patra’s COVID-19 Food Relief Service",
        text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris. Lorem ipsum dolor sit amet, consectetur. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris quis aliquam. Integer accumsan sodales odio, id tempus velit ullamc.",
        btn: "Read more",
        img: "4.png",
      },
      {
        title: "73rd International Human Rights Day Observed",
        text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris. Lorem ipsum dolor sit amet, consectetur. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris quis aliquam. Integer accumsan sodales odio, id tempus velit ullamc.",
        btn: "Read more",
        img: "5.png",
      },
      {
        title: "National Civil Society Conference 2021 Concludes",
        text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris. Lorem ipsum dolor sit amet, consectetur. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris quis aliquam. Integer accumsan sodales odio, id tempus velit ullamc.",
        btn: "Read more",
        img: "2.png",
      },
    ],
  }),
};
</script>

<style>
</style>