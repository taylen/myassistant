<template>
    <div class="container">
        <div v-show="showIndex">
            <div>曾经多个晚上梦到高考的那段时光</div>
            <div>难道是我高考产生了阴影</div>
            <div>我从未觉得当时有多艰难</div>
            <div>那为什么我经常会梦到那段时光</div>
            <div>唯一的解释是那段时光很艰辛</div>
            <div>艰辛伴随着充实，充实让我收获良多</div>
            <div>现在太过于安逸和享受</div>
            <div>人无远虑，必有近忧</div>
            <div>年轻的时候要奋斗和坚持</div>
            <div>而不是浑浑噩噩度过这最美的年华</div>
            <div>拿出当年的拼劲奋斗十五年</div>
            <div>我坚信你同样收获良多！</div>
            <button class="weui-btn open" @click="openMySelf" type="primary">开启修身之路</button>
        </div>        
    </div>
</template>
<script>
export default {
  data () {
    return {
      showIndex: true
    }
  },
  methods: {
    openMySelf () {
      this.showIndex = false
    }
  }
}
</script>

<style scoped> 
.open {
    margin-top: 40rpx;
}
</style>
