<template>
    <view class="header">
        <text class="title">{{ title }}</text>
    </view>
</template>

<script>
export default {
    props: {
        title: { type: String },
    },
}
</script>

<style>
.header {
    height: 80px;
    background-color: #eee;
    justify-content: center;
    align-items: center;
}
.title {
    color: #646464;
    font-size: 32px;
    font-weight: 900;
    text-transform: uppercase;
}
</style>