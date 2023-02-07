<template>
  <div>
    <select name="" v-model="selectedCity">
      <option value=""></option>
      <option value="02">서울</option>
      <option value="051">부산</option>
      <option value="054">포항</option>
      <option value="064">제주</option>
    </select>

  </div>
</template>

<script>

export default {

  components: {},

  data() {
    return {
      selectedCity: '054'
    }
  },

  setup() {},

  created() {},

  mounted() {},

  unmounted() {},

  methods: {}

}

</script>

<style scoped>

</style>
