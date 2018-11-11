<template>
  <v-img
    :src="src"
    :width="width"
    :max-width="maxWidth"
    :height="height"
    :max-height="maxHeight"
    class="madeco-slide-preview"/>
</template>

<script>
export default {
  props: {
    src: {
      type: String,
      required: true
    },
    width: {
      type: [Number, String],
      default: ''
    },
    maxWidth: {
      type: [Number, String],
      default: ''
    },
    height: {
      type: [Number, String],
      default: ''
    },
    maxHeight: {
      type: [Number, String],
      default: ''
    }
  }
}
</script>

<style lang="scss" scoped>
.madeco-slide-preview {
  border-radius: 8px;
}
</style>
