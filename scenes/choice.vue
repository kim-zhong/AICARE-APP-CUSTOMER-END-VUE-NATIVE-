<template>
  
  <view class="container">
    <touchable-opacity >
      <image class = "arrow_image"
        :source="require('./assets/icon/icon/2/Arrow_left.png')"
      />
    </touchable-opacity> 

    <text class = "service">服务详情</text>
    <image class = "choice"
      :source = "require('./assets/icon/icon/2/choice.png')"
    />

    <touchable-opacity class="onsite-wrapper">
      <text class="onsite-text">上门做饭</text>
    </touchable-opacity> 

    <text class="caption">口味可自行挑选，一餐1-5道菜。</text>
    <view class ="switch_container">
      <switch class="tick1"
          :value="value"
          :onValueChange="handleChange"
        />
      <text class="switch_text">如需额外购买食材将收取$20。</text>
    </view>

    <touchable-opacity class="clean-wrapper">
      <text class="onsite-text">上门清洁</text>
    </touchable-opacity>
    <text class="caption2">包括地面，门窗，垃圾清洁等。</text>

    <touchable-opacity class="care-wrapper">
      <text class="onsite-text">照顾老/幼</text>
    </touchable-opacity>
    <text class="caption2">日常生活料理等。</text>
  
    <view class ="comment_container">
      <image class="comment"
          :source = "require('./assets/icon/icon/2/comment.png')"
        />
      <touchable-opacity >
      <image class = "comment_image"
        :source="require('./assets/icon/icon/2/Arrow_right.png')"
      />
    </touchable-opacity> 
    </view>
    <!--below should be v-for touchable instead of image. Need to fix in the later development-->
    <image class = "comments"
        :source="require('./assets/icon/icon/2/comments.png')"
    />
    <image class = "bottom"
        :source="require('./assets/icon/icon/2/bottom.png')"
    />
    <touchable-opacity class="next-wrapper">
      <text class="onsite-text">下一步</text>
    </touchable-opacity>

    <image class = "contact"
      :source = "require('./assets/icon/icon/1/contact.png')"
    />
  </view>

</template>

<script>

export default {
  data:function(){
    return{
      value:false
    }
  },
  methods:{
    handleChange:function(val){
      this.value=val;
    }
  }
  
}
</script>

<style>
.contact{
  width:220;
  height:30;
  margin-left:100;
  margin-top:15;
}
.bottom{
  margin-top:90;
  margin-left:50;
}
.comments{
  margin-left:30;
  margin-top:10;
  height:40;
}
.switch_text{
  margin-top:16;
  font-size:11;
  color:#999999;
}
.switch_container{
  flex-direction:row;
}

.comment_container{
  flex-direction:row;
  margin-top:30;
}
.tick1{
  margin-left:40;
  margin-top:10;
}
.caption2{
  font-size:12;
  margin-left:50;
  margin-top:10;
}
.caption{
  font-size:12;
  margin-left:50;
  margin-top:10;
}

.arrow_image{
  width:25;
  height:25;
  margin-top:20;
  margin-left:20;
}
.comment_image{
  width:25;
  height:25;
  margin-top:20;
  margin-left:20;
}
.comment{
  width:100;
  height:25;
  margin-top:20;
  margin-left:50;
}
.container {
  background-color: white;
  margin-top: 35;
  flex: 1;
}

.service{
  color:#006A71;
  font-size:16;
  margin-top:20;
  margin-left:160;
}

.choice{
  margin-top:20;
  margin-left:40;
}

.clean-wrapper{
  backgroundColor:#8FD7D3;
  padding:10;
  width:120;
  margin-left:40;
  margin-top:25;
  height:45;
  align-items: center;
  borderRadius:10;
}
.next-wrapper{
  backgroundColor:#8FD7D3;
  padding:10;
  width:220;
  margin-left:100;
  margin-top:15;
  height:45;
  align-items: center;
  borderRadius:25;
}
.care-wrapper{
  backgroundColor:#8FD7D3;
  padding:10;
  width:120;
  margin-left:40;
  margin-top:25;
  height:45;
  align-items: center;
  borderRadius:10;
}
.onsite-wrapper{
  backgroundColor:#8FD7D3;
  padding:10;
  width:120;
  margin-left:40;
  margin-top:10;
  height:45;
  align-items: center;
  borderRadius:10;
}

.onsite-text{
  color:white;
}
</style>

