<template>
  <div>
    <home-header></home-header>
    <home-nav></home-nav>
    <home-wrap></home-wrap>
  </div>
</template>
<script>
import HomeHeader from './Header/Header'
import HomeNav from './Nav/Nav'
import HomeWrap from './Wrap/Wrap'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeNav,
    HomeWrap
  }
}
</script>
<style>

</style>
