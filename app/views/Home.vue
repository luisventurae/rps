<template>
  <view class="container">
    <StatusBar :bg_color="bg_color" />
    <Header :title="title" />
    <view class="input-container"> 
        <text-input class="input" placeholder="Nombre de Usuario" v-model="username" />
        <touchable-opacity class="add-btn" :on-press="setUsername" >
            <text class="btn-text">SAVE</text>
        </touchable-opacity>
    </view>
    <view class="sets-container">
        <text class="set-text">{{ set.username }}</text>
    </view>
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
    username: null,
    set: {
        username: null,
    },
  }),
  methods: {
      async setUsername() {
          this.set.username = this.username
          this.username = null
      },
  },
}
</script>

<style>
.container {
  background-color: white;
  flex: 1;
}
.input-container {
    flex-direction: row;
    justify-content: center;
    align-content: center;
}
.input {
    flex: 1;
    height: 35px;
    border-color: gray;
    font-size: 20px;
    padding: 5px;
    color: #646464;
}
.add-btn {
    width: 100px;
    height: 35px;
    background-color: #f39c12;
    padding: 15px;
    justify-content: center;
    align-content: center;

}
.btn-text {
    font-size: 20px;
    font-weight: 700;
    color: #fff;
}
.set-text {
    width: 100%;
    font-size: 40px;
    justify-content: center;
    align-content: center;
}
</style>