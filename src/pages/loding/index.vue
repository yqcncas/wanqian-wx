<template>
   <div class="load-page">
        <div class="outer-load center-box"></div>
        <image class="inner-load center-box" src="/static/images/logo.png"></image>
  </div>
</template>

<script>
export default {
  data () {
    return {
    }
  }
}
</script>

<style lang='less' scoped>
.load-page {
    width: 100%;
    height: 100%;
    background-color: #fff;
    position: relative;
  }
  .center-box {
    position: absolute;
    top: 50%;
    left: 50%;
  }
  .outer-load {
    border: ~'10rpx' solid #2b93ec;
    opacity: 0.9;
    width: ~'200rpx';
    height: ~'200rpx';
    border-top-color: transparent;
    border-bottom-color: transparent;
    border-radius: 50%;
    animation: spin-right 0.8s linear infinite normal;
    animation-delay: 0s;
    margin-left: ~'-110rpx';
    margin-top: ~'-200rpx';
  }
  @keyframes spin-right {
    0% {
      transform: rotate(0deg);
      opacity: 0.2;
    }

    50% {
      transform: rotate(180deg);
      opacity: 1;
    }

    100% {
      transform: rotate(360deg);
      opacity: 0.2;
    }
  }
  .inner-load {
    display: block;
    width: ~'100rpx';
    height: ~'100rpx';
    opacity: 0.9;
    margin-left: ~'-50rpx';
    margin-top: ~'-145rpx';
  }
  @keyframes spin-left {
    0% {
      transform: rotate(0deg);
      opacity: 0.2;
    }

    50% {
      transform: rotate(-180deg);
      opacity: 1;
    }

    100% {
      transform: rotate(-360deg);
      opacity: 0.2;
    }
  }
</style>
