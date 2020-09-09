<template>
  <div id="app">
    <FirstScreen />
    <AboutUs />
    <OurFriends />
    <YouCanHelp />
    <Donation />
  </div>
</template>

<script>

import FirstScreen from './components/FirstScreen/FirstScreen'
import AboutUs from './components/AboutUs/AboutUs'
import OurFriends from './components/OurFriends/OurFriends'
import YouCanHelp from './components/YouCanHelp/YouCanHelp'
import Donation from './components/Donation/Donation'
export default {
  name: 'App',
  components: { Donation, YouCanHelp, OurFriends, AboutUs, FirstScreen }
}
</script>

<style lang="scss">
  @import 'assets/scss/main.scss';
</style>
