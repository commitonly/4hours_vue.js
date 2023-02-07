<template>
  <div>
    <div> {{ htmlString }}</div>
    <!-- 문자열이 아닌 html 태그로 추가하는 방법 -->
    <div v-html="htmlString"></div>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      htmlString: '<p style="color:red;">빨간색문자</p>'
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
