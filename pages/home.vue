<template>
  <div>
   
    <donate />
    <together />
    <upcoming />
    <urgent />
    <latest />
  </div>
</template>

<script>
import Donate from "../components/donate.vue";
import Latest from '../components/latest.vue';
import Together from "../components/together.vue";
import Upcoming from "../components/upcoming.vue";
import urgent from "../components/urgent.vue";
export default {
  components: { urgent, Donate, Together, Upcoming, Latest },
  
};
</script>

<style>
</style>