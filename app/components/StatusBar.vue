<template>
    <view class="status-bar" :style="{ backgroundColor: bg_color}" ></view>
</template>

<script>
export default {
    props: {
        bg_color: { type: String }
    },
}
</script>

<style>
.status-bar {
    height: 40px;
}
</style>