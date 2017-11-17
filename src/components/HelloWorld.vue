<template>
  <div>
    Hello, {{text | upper}}
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'HelloWorld',
  components: {
  },
  props: {
    text: {
      type: String,
      required: true,
      default: ''
    }
  },
  filters: {
    upper (text: string): string {
      return text.toUpperCase()
    }
  }
})
</script>

<style>
</style>
