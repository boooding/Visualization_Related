<template>
  <common-card
    title="Total Order Number"
    value="20,212"
  >
    <template>
    </template>
    <template v-slot:footer>
      <span>Order Number Last day </span>
      <span class="emphasis">{{orderLastDay}}</span>
    </template>
  </common-card>
</template>

<script>
import CommonCard from '../CommonCard'
import commonCardMixin from '../../../mixins/commonCardMixin'

export default {
  name: 'TotalOrders',
  mixins: [commonCardMixin],
  comments: {
    CommonCard
  }
}
</script>

<style scoped>

</style>
