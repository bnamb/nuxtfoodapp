<template>
  <div>
    <label :for="select">WhichPaul {{ select }} would you like?</label>

    <!-- <select @change="emit('change', event.target.value)" :id="select" :name="select"> -->
    <!-- <select @change="onChange($event)" :id="select" :name="select">
      <option value>-- Please select a {{ select }} --</option>
      <option v-for="option in selectOptions" :key="option" value="option">
        {{option}}
        </option>
    </select> -->
    <button @click="name = 'Steven B'">Change Name</button>
    <select name="LeaveType" @change="greet" class="form-control">
      <option value="1">Annual Leave/ Off-Day</option>
      <option value="2">On Demand Leave</option>
    </select>
    {{name}}

  </div>
</template>

<script>
  export default {
    data() {
      return {
        name: "Paul"
      }
    },
    props: {
      select: {
        type: String,
        default: "cuisine",
      },
      selectOptions: {
        type: Array,
        default: () => ["tacos", "pizza", "dimsum"],
      },
    },
    methods: {
        onChange(event) {
            console.log(event.target.value)
        },
         greet() {
          // `this` inside methods points to the current active instance
          alert('Hello');
        }
    }
  }
</script>

<style lang="scss" scoped>

</style>
