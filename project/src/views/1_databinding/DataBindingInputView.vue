<template>
  <div>
    <input type="text" v-model="userId" />
    <button @click="myFunction">클릭</button>
    <button @click="changeData">변경</button>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      userId: 'taemin.kim'
    }
  },
  setup() {},
  created() {},
  mounted() {},
  unmounted() {},
  methods: {
    myFunction() {
      console.log(this.userId)
    },
    changeData() {
      this.userId = 'tem'
    }
  }
}
</script>

<style scoped>

</style>
