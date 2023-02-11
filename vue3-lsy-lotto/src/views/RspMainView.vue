<template>
  <lotto-header></lotto-header>
  <RspMain></RspMain>
  <lotto-footer></lotto-footer>
</template>

<script>
import LottoFooter from '../components/LottoFooter.vue'
import LottoHeader from '../components/LottoHeader.vue'
import RspMain from '@/components/rsp/RspMain.vue'

export default {
  name: 'LottoMainView',
  components: {
    LottoFooter,
    LottoHeader,
    RspMain
  }
}
</script>

<style scoped></style>
