<template>
  <div class="hearder">
    <img  class="hearderimg"  src="/static/images/details.png" >
    <text class="heardertext">轻落，一点一点消融。遥望中，一丝一丝心痛。花落花开开不休，上善若水水自流。红颜远，相思苦，几番意，难相付。</text>
  </div>
</template>

<script>
export default {
  
}
</script>
<style lang="scss" scoped>
  @import "static/style/common.scss";
  .hearder{
     width: 100%;
     height: 360rpx;
    .hearderimg{
      width: 100%;
      height: 100%;
    }
    .heardertext{
       position: absolute;
       top: 235rpx;
       color:rgb(65, 40, 209);
       font-size: 16px;
       margin: auto 36rpx;
       @include ellipsis-row(2);
    }
  }
</style>
