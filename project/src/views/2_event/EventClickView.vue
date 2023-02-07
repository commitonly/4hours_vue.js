<template>
  <div>
    <button @click="increaseCounter">Add 1</button>
    <p>{{ counter }}</p>
    <button @click="decreaseCounter">Delete 1</button>

  </div>
</template>

<script>

export default {

  components: {},

  data() {
    return {
      counter: 0
    }
  },

  setup() {},

  created() {},

  mounted() {},

  unmounted() {},

  methods: {
    increaseCounter() {
      this.counter += 1
    },
    decreaseCounter() {
      this.counter -= 1
    }
  }

}

</script>

<style scoped>

</style>
