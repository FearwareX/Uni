<template>
  <view class="content">
    <image class="logo" src="/static/logo.png"></image>
    <view>
      <text class="title">{{ title }}</text>
    </view>
    <text>
      {{ $u.timeFormat(new Date().valueOf(), 'yyyy年mm月dd日hh:MM:ss') }}
    </text>
  </view>
</template>

<script>
export default {
  data() {
    return {
      title: 'HelloWorld',
    };
  },
  onLoad() {
    console.log(this.title);
  },
  methods: {},
};
</script>

<style lang="scss">
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.logo {
  width: 200rpx;
  height: 200rpx;
  margin: 200rpx auto 50rpx auto;
}

.title {
  font-size: 36rpx;
  color: #8f8f94;
}
</style>
