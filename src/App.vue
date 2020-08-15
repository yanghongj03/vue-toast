<template>
  <div id="app">
    <button @click="showToast">点我哦</button>
  </div>
</template>

<script>

export default {
  name: 'App',
  methods: {
    showToast () {
      this.$toast()
    }
  }
}
</script>

<style>
body {
  height: 100%;
  width: 100%;
}
#app {
  height: 100%;
  width: 100%;
}
</style>
