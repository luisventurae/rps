<template>
  <view class="container">
    <StatusBar :bg_color="bg_color" />
    <Header :title="title" />
    <!-- <Home /> -->
  </view>
</template>

<script>
import StatusBar from './app/components/StatusBar'
import Header from './app/components/Header'
import Home from './app/components/Home'

export default {
  components: {
    StatusBar,
    Header,
    Home,
  },
  data: () => ({
    bg_color: '#f39c12',
    title: 'RPS',
  }),
}
</script>

<style>
.container {
  background-color: white;
  flex: 1;
}
</style>
