<template>
  <div>
    <v-img src="13.png">
      <v-row justify="center">
        <h1 class="white--text" style="font-size: 72px; margin-top: 120px">
          Causes
        </h1>
      </v-row>
    </v-img>

    <urgent />
    <othercauses />
  </div>
</template>

<script>
import Othercauses from "../components/othercauses.vue";

import teammember from "../components/teammember.vue";
import Urgent from "../components/urgent.vue";
export default {
  components: { teammember, Urgent, Othercauses },
  data: () => ({
    links: [
      {
        img: "1.jpg",
        title: "About Our NGO",
        text: "Lorem ipsum dolor sit amet, con sectetur adipiscing elit. Mauris temp us vestib ulum mauris.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris.Lorem ipsum dolo.Lorem ipsum dolor sit amet, con sectetur adipiscing elit. Mauris temp us vestib ulum mauris.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris tempus vestib ulum mauris.Lorem ipsum dolo..........",
      },
    ],
  }),
};
</script>

<style>
</style>