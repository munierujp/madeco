<template>
  <v-btn
    :color="color"
    :href="href"
    :to="to"
    dark
    class="madeco-download-button">
    <v-icon
      left
      dark>cloud_download</v-icon>
    {{ label }}
  </v-btn>
</template>

<script>
export default {
  props: {
    color: {
      type: String,
      required: true
    },
    label: {
      type: String,
      required: true
    },
    href: {
      type: String,
      default: ''
    },
    to: {
      type: String,
      default: ''
    }
  }
}
</script>

<style lang="scss" scoped>
.madeco-download-button {
  text-transform: none;
}
</style>
