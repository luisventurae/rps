<template>
  <view class="container">
    <StatusBar :bg_color="bg_color" />
    <Header :title="title" />
  </view>
</template>

<script>
import StatusBar from '../components/StatusBar'
import Header from '../components/Header'

export default {
  components: {
    StatusBar,
    Header,
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