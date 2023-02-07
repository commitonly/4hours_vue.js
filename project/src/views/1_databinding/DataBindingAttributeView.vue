<template>
  <div>
    <input type="text" name="" id="" v-bind:value="userId" readonly>
    <input type="text" name="" id="" :value="userId" readonly>
    <br/> <br/>
    <img :src="imgSrc" alt="" style="width: 100px; height: auto;">
  </div>
  <br/>
  <input type="search" name="" id="" v-model="txt1">
  <button :disabled="txt1 === '' ">조회</button>
</template>

<script>

export default {

  components: {},

  data() {
    return {
      userId: 'TaeminKim',
      imgSrc: 'https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/1200px-Vue.js_Logo_2.svg.png',
      txt1: ''
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
