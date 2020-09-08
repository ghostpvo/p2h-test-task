<template>
  <div id="app">
    <FirstScreen />
  </div>
</template>

<script>

import FirstScreen from './components/FirstScreen/FirstScreen'
export default {
  name: 'App',
  components: { FirstScreen }
}
</script>

<style lang="scss">
  @import 'assets/scss/main.scss';
</style>
