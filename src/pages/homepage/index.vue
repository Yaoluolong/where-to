<template>
  <div>
    <home-header></home-header>
    <home-nav></home-nav>
  </div>
</template>
<script>
import HomeHeader from './Header/Header'
import HomeNav from './Nav/Nav'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeNav
  }
}
</script>
<style>

</style>
