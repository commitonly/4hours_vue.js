<template>
  <div>
    <div>
      <input type="checkbox" name="" id="html" value="HTML" v-model="favoriteLang">
      <label for="html">HTML</label>
    </div>
    <div>
      <input type="checkbox" name="" id="css" value="CSS" v-model="favoriteLang">
      <label for="css">CSS</label>
      <div>
        <input type="checkbox" name="" id="js" value="JavaScript" v-model="favoriteLang">
        <label for="js">JS</label>
        <div>선택한 지역: {{ favoriteLang }}</div>
      </div>
    </div>
  </div>
</template>

<script>

export default {

  components: {},

  data() {
    return {
      favoriteLang: ['JS']
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
