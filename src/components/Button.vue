<template>
  <button
    class="btn btn-warning btn-lg text-dark fw-bold rounded-0 w-100 position-sticky bottom-0"
    v-if="isShow"
  >贊助專案</button>
</template>
<script>
export default {
  props: ['height'],
  data () {
    return {
      isShow: false
    }
  },
  watch: {
    height: function (value) {
      if (value > 530 && value < 3550) {
        this.isShow = true
      } else {
        this.isShow = false
      }
    }
  }
}
</script>