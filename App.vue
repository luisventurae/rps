<template>
  <view class="container">
    <Home />
  </view>
</template>

<script>
import Home from './app/views/Home'

export default {
  components: {
    Home,
  },
}
</script>

<style>
.container {
  background-color: white;
  flex: 1;
}
</style>
