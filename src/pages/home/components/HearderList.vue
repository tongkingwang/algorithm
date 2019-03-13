<template>
  <div>
    <div class="hearderlist" @click="handleEnter(item.id)" v-for="(item, index) of List" :key="index">
        <img class="hearderlistimgtwo" :src="item.listimg">
      <div class="hearderlisttext">
        <div class="headerlisttextone"><text>{{item.title}}</text></div>
        <div class="hearderlisttexttwo">
              <div class="hearderend">{{item.author}}</div>
              <div class="handerend">{{item.date}}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      List:[
        {
          id:1,
          listimg:'/static/images/scenery.png',
          title:'我愿意深深地扎入生活，吮尽生活的骨髓，过得扎实，简单，把一切不属于生活的内容剔除得干净利落，把生活逼到绝处，用最基本的形式，简单，简单，再简单...',
          author:'王彦兴',
          date:'35分钟前'
        },
        {
          id:2,
          listimg:'/static/images/scenery.png',
          title:'我愿意深深地扎入生活，吮尽生活的骨髓，过得扎实，简单，把一切不属于生活的内容剔除得干净利落，把生活逼到绝处，用最基本的形式，简单，简单，再简单...',
          author:'王彦兴',
          date:'35分钟前'
        },
        {
          id:3,
          listimg:'/static/images/scenery.png',
          title:'我愿意深深地扎入生活，吮尽生活的骨髓，过得扎实，简单，把一切不属于生活的内容剔除得干净利落，把生活逼到绝处，用最基本的形式，简单，简单，再简单...',
          author:'王彦兴',
          date:'35分钟前'
        },
        {
          id:4,
          listimg:'/static/images/scenery.png',
          title:'我愿意深深地扎入生活，吮尽生活的骨髓，过得扎实，简单，把一切不属于生活的内容剔除得干净利落，把生活逼到绝处，用最基本的形式，简单，简单，再简单...',
          author:'王彦兴',
          date:'35分钟前'
        },
        {
          id:5,
          listimg:'/static/images/scenery.png',
          title:'我愿意深深地扎入生活，吮尽生活的骨髓，过得扎实，简单，把一切不属于生活的内容剔除得干净利落，把生活逼到绝处，用最基本的形式，简单，简单，再简单...',
          author:'王彦兴',
          date:'35分钟前'
        }, 
        {
          id:6,
          listimg:'/static/images/scenery.png',
          title:'我愿意深深地扎入生活，吮尽生活的骨髓，过得扎实，简单，把一切不属于生活的内容剔除得干净利落，把生活逼到绝处，用最基本的形式，简单，简单，再简单...',
          author:'王彦兴',
          date:'35分钟前'
        }


      ]


    };
  },
  methods: {
   
    handleEnter(id) {
  
      wx.navigateTo({
         url: `./homeDetail/main?id=${id}`
      });
    }
  }

}
</script>
<style lang="scss" scoped>
@import "static/style/common.scss";
.hearderlist{
  display: flex;
  flex-direction: row;
  width: auto;
  height: 160rpx;
  .hearderlistimgtwo{
    height: 100%;
    margin: 20rpx 8rpx 20rpx 25rpx;

  }
  .hearderlisttext{
    display: flex;
    flex-direction: column;
    height: 100%;
    .headerlisttextone{
      height: 100%;
      margin: 36rpx 50rpx 8rpx 12rpx;
      color: #000;
      font-size: 16px;
      @include ellipsis-row(2);
    }
    .hearderlisttexttwo{
      display:flex;
      flex-direction:row;
      .hearderend{
        color:#7b7980;
        font-size:14px;
        margin:auto auto 2rpx 12rpx;

      }
      .handerend{
        color:#7b7980;
        font-size:14px;
        margin-right:30rpx;
      }
    }

  }
}



</style>
