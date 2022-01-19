<template>
  <common-card
    title="Total sales"
    value="£ 50,502,223"
  >
    <template>
      <div class="compare-wrapper">
        <div class="compare">
          <span>Compare to last Day</span>
          <span class="emphasis">{{salesGrowthLastDay}}</span>
          <div class="increase" />
        </div>
        <div class="compare">
          <span>Compare to last Month</span>
          <span class="emphasis">{{salesGrowthLastMonth}}</span>
          <div class="decrease" />
        </div>
      </div>
    </template>
    <template v-slot:footer>
      <div>
        <span>
          Yesterday sales:
        </span>
        <span class="emphasis">
          £ 23,333
        </span>
      </div>
    </template>
  </common-card>
</template>

<script>
import commonCardMixin from '../../../mixins/commonCardMixin'
import CommonCard from '../CommonCard'

export default {
  name: 'TotalSales',
  mixins: [commonCardMixin],
  comments: {
    CommonCard
  }
}
</script>

<style scoped>
.compare-wrapper {
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.compare-wrapper .compare {
  display: flex;
  align-items: center;
  font-size: 12px;
  margin-top: 3px;
  color: #666;
}
</style>
