<template>
  <div id="app">
    <FirstScreen />
    <AboutUs />
    <OurFriends />
  </div>
</template>

<script>

import FirstScreen from './components/FirstScreen/FirstScreen'
import AboutUs from './components/AboutUs/AboutUs'
import OurFriends from './components/OurFriends/OurFriends'
export default {
  name: 'App',
  components: { OurFriends, AboutUs, FirstScreen }
}
</script>

<style lang="scss">
  @import 'assets/scss/main.scss';
</style>
