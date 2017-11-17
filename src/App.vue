<template>
  <div id="app">
    <hello-world
      :text="'world'"
    ></hello-world>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import HelloWorld from '@/components/HelloWorld.vue'

export default Vue.extend({
  name: 'app',
  components: {
    HelloWorld
  },
  props: {
    size: {
      type: Number,
      required: false,
      default: 10
    }
  },
  computed: {
    halfSize (): number {
      return this.size / 2
    }
  }
})
</script>

<style>
</style>
