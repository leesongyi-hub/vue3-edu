<template>
  <lotto-header></lotto-header>
  <lotto-main></lotto-main>
  <lotto-footer></lotto-footer>
</template>

<script>
import LottoFooter from '../components/LottoFooter.vue'
import LottoHeader from '../components/LottoHeader.vue'
import LottoMain from '../components/LottoMain.vue'

export default {
  name: 'LottoMainView',
  components: {
    LottoFooter,
    LottoHeader,
    LottoMain
  }
}
</script>

<style scoped></style>
