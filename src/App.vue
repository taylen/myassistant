<script>
export default {
  created () {
    wx.cloud.init()

    // 调用API从本地缓存中获取数据
    const logs = wx.getStorageSync('logs') || []
    logs.unshift(Date.now())
    wx.setStorageSync('logs', logs)

    wx.showToast({
      title: 'app created and cache logs by setStorageSync'
    })
  }
}
</script>

<style>
@import '../static/style/weui.wxss';

.container {
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  padding: 50rpx 10rpx;
  box-sizing: border-box;
  font-size: 35rpx;
}
/* this rule will be remove */
* {
  transition: width 2s;
  -moz-transition: width 2s;
  -webkit-transition: width 2s;
  -o-transition: width 2s;
}
</style>
