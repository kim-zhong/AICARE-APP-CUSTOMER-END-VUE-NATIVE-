<template>
  <view class = "container">
    <image class = "img"  
      :source = "require('./assets/consumer/icon/welcome.png')"
    />
    <image class = "img_ac"  
      :source = "require('./assets/consumer/icon/account.png')"
    />
    <text-input class = "account"/>
    <image class = "img_pw"  
      :source = "require('./assets/consumer/icon/password.png')"
    />
    <text-input class = "password"/>
    <view class ="container2">
      <touchable-opacity class="f-wrapper">
        <text class="f-text">忘记密码？</text>
      </touchable-opacity>
      <touchable-opacity class="f-wrapper">
        <text class="r-text">注册账户</text>
      </touchable-opacity>
    </view>
    <touchable-opacity class="login-wrapper">
      <text class="onsite-text">登陆</text>
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
.r-text{
  color:#333333;
  margin-left:145;
}
.f-text{
  color:#333333;
  margin-left:0;

}
.f-wrapper{
  margin-top:20;
}

.container2{
  flex-direction:row;
}
.login-wrapper{
  backgroundColor:#8FD7D3;
  padding:10;
  width:240;
  margin-top:60;
  height:45;
  align-items: center;
  borderRadius:25;
}
.img_ac{
  height:30;
  width:300;
  margin-top:40;
}
.img_pw{
  margin-top:30;
  height:30;
  width:300;
}
.account{
  height: 35;
  width: 300;
  borderBottomColor:#999999;
  borderBottomWidth:1;
}
.password{
  height: 35;
  width: 300;
  borderBottomColor:#999999;
  borderBottomWidth:1;
}
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
  margin-top:90;
  width:300;
  height:300;


}
</style>