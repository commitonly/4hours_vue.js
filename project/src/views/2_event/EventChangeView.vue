<template>
  <div>
    <!--        <select name="" id="" @change="changeCity" v-model="selectedCity">-->
    <!--    약자는 @ 이지만 하단에서처럼 v-on 으로 사용할 수 있다 -->
    <!--    @ == v-on , : == v-bind 이렇게 알고 있으면 된다. -->
    <select name="" id="" v-on:change="changeCity" v-model="selectedCity">
      <!--    하단에서 직접 필터를 사용했을 경우 위에서처럼 체인지를 따로 쓰지 않아도 될 만큼 뷰는 강력하다 -->
      <!--    <select name="" id="" v-model="selectedCity">-->
      <option value="">==도시선택==</option>
      <option
        :value="city.cityCode"
        :key=city.cityCode
        v-for="city in cityList"
      >
        {{ city.title }}
      </option>
    </select>
    <select name="" id="">
      <option
        :value="dong.dongCode"
        :key="dong.dongCode"
        v-for="dong in selectedDongList"
      >
        {{ dong.dongTitle }}
      </option>
    </select>
    <!--    <select name="" id="">-->
    <!--      <option-->
    <!--        :value="dong.dongCode"-->
    <!--        :key="dong.dongCode"-->
    <!--        v-for="dong in dongList.filter(-->
    <!--          (dong) => dong.cityCode === selectedCity-->
    <!--        )"-->
    <!--      >-->
    <!--        {{ dong.dongTitle }}-->
    <!--      </option>-->
    <!--    </select>-->
  </div>
</template>

<script>

export default {

  components: {},

  data() {
    return {
      selectedCity :'',
      cityList: [
        { cityCode: '02', title: '서울' },
        { cityCode: '051', title: '부산' },
        { cityCode: '064', title: '제주도' }
      ],
      dongList: [
        { cityCode: '02', dongCode: '1', dongTitle: '서울 1동' },
        { cityCode: '02', dongCode: '2', dongTitle: '서울 2동' },
        { cityCode: '02', dongCode: '3', dongTitle: '서울 3동' },
        { cityCode: '02', dongCode: '4', dongTitle: '서울 4동' },
        { cityCode: '051', dongCode: '1', dongTitle: '부산 1동' },
        { cityCode: '051', dongCode: '2', dongTitle: '부산 2동' },
        { cityCode: '051', dongCode: '3', dongTitle: '부산 3동' },
        { cityCode: '051', dongCode: '4', dongTitle: '부산 4동' },
        { cityCode: '064', dongCode: '1', dongTitle: '제주 1동' },
        { cityCode: '064', dongCode: '2', dongTitle: '제주 2동' }
      ],
      selectedDongList: []
    }
  },

  setup() {},

  created() {},

  mounted() {},

  unmounted() {},

  methods: {
    changeCity() {
      this.selectedDongList = this.dongList.filter( (dong) => dong.cityCode === this.selectedCity)
    }
  }

}

</script>

<style scoped>

</style>
