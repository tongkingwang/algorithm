<template>
  <div class="detail-container">
    <hearder-home/>
    <div class="detail-syn">小明<text>发布于</text>12小时前</div>
    <div class="content" >
          <text space="nbsp" decode >
            三月，醉一场青春的流年。慢步在三月的春光里，走走停停，看花开嫣然，看春雨绵绵，感受春风拂面，春天，就是青春的流年。青春，是人生中最美的风景。青春，是一场花开的遇见；青春，是一场痛并快乐着的旅行；青春，是一场轰轰烈烈的比赛；青春，是一场鲜衣奴马的争荣岁月；青春，是一场风花雪月的光阴。
          </text>

    </div>
  </div>
</template>
<script>
import HearderHome from '../components/HearderHome'
export default {
  components:{
    HearderHome
  },
  onLoad(option) {
    console.log("接收id", option.id);
  }

}
</script>

<style>


</style>
