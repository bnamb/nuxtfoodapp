<template>
<main class="container restaurant">
  <div class="restaurantheading">
    <h1>Restaurant List</h1>
        <button @click="alert('hi')">Change Name</button>
          <AppSelect @change="selectedRestaurant = $event"/>
          <!-- <pre> {{ $event }} Steven3 </pre> -->

  </div>
      <AppRestaurantInfo />
</main>
</template>

<script>
  import AppRestaurantInfo from '@/components/AppRestaurantInfo.vue';
  import AppSelect from '@/components/AppSelect.vue';

  export default {
    components: {
      AppSelect,
      AppRestaurantInfo
    },
    data() {
      return {
        selectedRestaurant: "",
      }
    },
  };
</script>

<style lang="scss" scoped>
h1 {
  text-align: center;
  padding: 0px;
  font-size: 5vmax;
}
</style>
