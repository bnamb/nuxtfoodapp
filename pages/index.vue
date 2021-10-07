<template>
  <main class="container restaurant">
    <AppHeader />
    <AppRestaurantInfo />
  </main>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue';
import AppRestaurantInfo from '@/components/AppRestaurantInfo.vue';

export default {
  components: {
    AppRestaurantInfo,
    AppHeader,
  },
};
</script>

<style>

</style>
