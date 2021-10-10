<template>
  <main class="container">
    <AppHeader />
    <!-- <AppRestaurantInfo :datasource="filteredRestaurants" /> -->
  </main>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue';
// import AppRestaurantInfo from '@/components/AppRestaurantInfo.vue';

export default {
  components: {
    // AppRestaurantInfo,
    AppHeader,
  },
};
</script>

<style>

</style>
