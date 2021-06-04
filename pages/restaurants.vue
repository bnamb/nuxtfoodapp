<template>
  <div>
    <h1>Restaurant List</h1>
    <AppRestaurantInfo />
  </div>
</template>

<script>
  import AppRestaurantInfo from '@/components/AppRestaurantInfo.vue';

  export default {
    components: {
      AppRestaurantInfo
    },
  };
</script>

<style lang="scss" scoped>
h1 {
  text-align: center;
  padding: 30px;
  font-size: 5vmax;
}
</style>
