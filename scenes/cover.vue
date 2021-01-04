<template>
  <view class = "container">
    <image class = "img"  
      :source = "require('./assets/consumer/icon/big.png')"
    />
    <touchable-opacity class="consumer-wrapper">
      <text class="onsite-text">我是消费者</text>
    </touchable-opacity> 
    <touchable-opacity class="provider-wrapper">
      <text class="onsite-text">我是服务者</text>
    </touchable-opacity> 

    <image class = "img2"  
      :source = "require('./assets/consumer/icon/logo.png')"
    />
  </view>
</template>

<script>
export default {
 
  
}
</script>

<style>
.onsite-text{
  color:white;
}
.container{
  background-color: white;
  margin-top: 20;
  flex: 1;
  align-items:center;
}
.consumer-wrapper{
  backgroundColor:#8FD7D3;
  padding:10;
  width:280;
  margin-top:60;
  height:45;
  align-items: center;
  borderRadius:25;
}
.provider-wrapper{
  backgroundColor:#FDB0A8;
  padding:10;
  width:280;
  margin-top:30;
  height:45;
  align-items: center;
  borderRadius:25;
}

.img2{
  margin-top:70;
  width:120;
  height:32;
}
.img{
  margin-top:30;
  width:380;
  height:500;


}
</style>