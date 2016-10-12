<template>
  <button class="button is-info" @click.prevent="activate">+1</button>
</template>

<script>
import store from '../store'

export default {
  data () {
    return {
      sharedState: store.state
    }
  },
  methods: {
    activate () {
      store.commit('INCREMENT')
    }
  }
}
</script>

<style>
</style>