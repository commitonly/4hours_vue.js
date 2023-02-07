<template>
  <div>
    <h1>Hello {{ userName }}</h1>
    <p> {{ message }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userName: 'Taemin Kim',
      message: 'Welcome Vue Js!',
      arr: [],
      ob: {}
    }
  }
}
</script>

<style lang="scss" scoped>
.text-red {
  color: red;
}
</style>
