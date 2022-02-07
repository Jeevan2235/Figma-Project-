<template>
  <div>
    <v-img src="9.png" > </v-img>

  <v-container>
      <v-row>
      <v-col cols="12" md="6" v-for="link in links" :key="link">
        <v-card-title class="text-h3">{{ link.title }}</v-card-title>
        <v-card-text style="font-size: 20px">{{ link.text }}</v-card-text>

        <v-list-item v-for="(item, i) in items" :key="i">
          <v-list-item-icon>
            <v-icon v-text="item.icon" color="#f94f19"></v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title v-text="item.text"></v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-row>
          <v-icon color="#f94f19" class="ma-5 ml-7">mdi-facebook</v-icon>
          <v-icon color="#f94f19" class="ma-3">mdi-twitter</v-icon>
          <v-icon color="#f94f19" class="ma-3">mdi-linkedin</v-icon>
          <v-icon color="#f94f19" class="ma-3">mdi-youtube</v-icon>
        </v-row>
      </v-col>
      <v-col cols="12" md="6">
        <v-card  class="pa-12" color="#e5e5e5" tile elevation="0">
          <v-text-field label="Name" solo></v-text-field>
          <v-text-field label="Email" solo></v-text-field>
          <v-textarea label="Message......" color="white" solo></v-textarea>
          <div class="text-center">
            <v-btn
              color="#f94f19"
              rounded
              elevation="0"
              height="2.5em"
              class="white--text"
              width="9em"
              >Contact Us</v-btn
            >
          </div>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
  </div>
</template>
       

<script>
export default {
  data: () => ({
    selectedItem: 1,
    items: [
      { text: "+977-9876548976", icon: "mdi-phone" },
      { text: "asd@gmail.com", icon: "mdi-email" },
      { text: "Gyaneshwor, Kathmandu", icon: "mdi-map-marker" },
    ],

    links: [
      {
        title: "Get in Touch with us",
        text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris.",
      },
    ],
  }),
};
</script>
<style>
</style>