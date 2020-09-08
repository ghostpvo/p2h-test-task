<template>
  <div id="app">

    <Header />
    <FirstScreen />
  </div>
</template>

<script>

import Header from './components/Header/Header'
import FirstScreen from './components/MainOffer/MainOffer'
export default {
  name: 'App',
  components: { Header, FirstScreen }
}
</script>

<style lang="scss">
  @import 'assets/scss/main.scss';
</style>
