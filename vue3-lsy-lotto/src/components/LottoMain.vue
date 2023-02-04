<template>
  <body>
    <div class="container">
      <div class="row mt-sm-5">
        <lotto-ball v-for="num in lottoSet" :key="num" :lottoNum="num"></lotto-ball>
      </div>
    </div>
  </body>
</template>

<script>
// @ is an alias to /src
import LottoBall from '@/components/LottoBall.vue'

export default {
  name: 'LottoMain',
  components: {
    LottoBall
  },
  data() {
    return { lottoSet: new Set() }
  },
  created() {
    console.log(typeof this.lottoSet)

    while (this.lottoSet.size != 6) {
      const lottoNum = Math.ceil(Math.random() * 45) //1부터 45까지 소수점빼고 변수에 저장
      this.lottoSet.add(lottoNum)
    }

    for (let temp of this.lottoSet) {
      console.log(temp)
    }
  }
}
</script>

<style scoped>
body {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
</style>
