<template>
  <common-card/>
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
