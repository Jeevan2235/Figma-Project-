<template>
  <div>
    <v-navigation-drawer v-model="drawer" temporary app right color="#0c2059">
      <h2 class="pa-2 white--text text-center" v-for="i in ['Home', 'About Us','Causes','Gallery','News', 'Contact', 'Donate']" :key="i">{{ i }}</h2 >
    </v-navigation-drawer>
    <v-row no-gutters class="mt-3">
      <v-card-title>
        <v-img class="ml-16" src="logo.png" height="40" width="70"></v-img>
      </v-card-title>
      <v-spacer></v-spacer>
      <div v-if="!isSmallEnough">
        <v-btn
          v-for="link in links"
          :key="link"
          text
          rounded
          class="mx-5 mt-3"
         
          link
          :to="i == 0 ? '/' : '/' + link.toLowerCase()"
        >
          {{ link }}
        </v-btn>
        <v-btn
          class="mt-3 white--text"
          color="#f94f19"
          rounded
          elevation="0"
          height="2.5em"
          width="9em"
          to="/donation"
        >
          Donate</v-btn
        >
        <v-icon class=" mt-3 mr-15 ml-5">mdi-magnify</v-icon>
      </div>
      <v-app-bar-nav-icon
        v-else
        class="mt-4"
        @click="drawer = !drawer"
      ></v-app-bar-nav-icon>
    </v-row>
  </div>
</template>

<script>
export default {
  methods: {
    onResize() {
      this.windowSize = { x: window.innerWidth, y: window.innerHeight };
    },
  },
  mounted() {
    this.onResize();
    window.addEventListener("resize", () => {
      this.onResize();
    });
  },
  computed: {
    isSmallEnough() {
      // return false
      return this.windowSize.x < 960 ? true : false;
    },
  },
  data: () => ({
    links: ["Home", "About Us", "Causes", "Gallery", "News", "Contact"],
    drawer: false,
    windowSize: {
      x: 0,
      y: 0,
    },
  }),
};
</script>

<style scoped>
</style>
