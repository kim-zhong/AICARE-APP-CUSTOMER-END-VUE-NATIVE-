
<template>
  
  <view class="container">


    <ImageBackground
        :style="{width: 138*3, height: 77*3,alignItems: 'center', backgroundColor: '#DDDDDD'}"
        :source="require('./assets/icon/icon/1/top.png')"
    >
      <view class = "image-text">
        <text class ="AICARE">AICARE</text>
        <text class = "slogon">为您提供最贴心的远程服务</text>
      </view>

    </ImageBackground>

    <text class ="title">请选择服务类型</text>

    <touchable-opacity :on-press="onPressButton" >
      <image class = "store_image"
        :source="require('./assets/icon/icon/1/store_image.png')"
      />
    </touchable-opacity> 

    <touchable-opacity :on-press="onPressButton" >
      <image class = "booking_image"
        :source="require('./assets/icon/icon/1/booking_image.png')"
      />
    </touchable-opacity>  

    <touchable-opacity :on-press="onPressButton" >
      <image class = "delivery_image"
        :source="require('./assets/icon/icon/1/delivery_image.png')"
      />
    </touchable-opacity> 

    <image class = "contact"
      :source = "require('./assets/icon/icon/1/contact.png')"
    />

  </view>
</template>

<script>
import { ImageBackground} from 'react-native';

export default {
  data() {
    return {
      message: "Hello World",
      value: false,
    };
  },
  methods: {
    exclaim() {
      this.message += "!";
    },
    onPressLearnMore: function() {
      alert('Hello')
    },
    handleChange: function(val) {
                this.value = val;
            },
    onPressButton: function() {
                alert('Clicked Image')
            },
  },

};
</script>

<style>
.container {
  background-color: white;
  align-items: center;
  margin-top: 35;
  flex: 1;
}


.store_image{
  margin-top:20;
  width:334;
  height:120;
}

.booking_image{
  margin-top:25;
  width:334;
  height:120;
}

.delivery_image{
  margin-top:25;
  width:334;
  height:120;
}

.contact{
  width:220;
  height:30;
  margin-top:50;
}

.title{
  color:#006A71;
  margin-top:60;
}

.AICARE{
  margin-top:100;
  margin-left:280;
  color:#006A71;
}

.slogon{
  margin-top:5;
  margin-left:192;
  color:white;
  font-size:10;
}

}
.button-image{
  width: 280;
  height:200;
  background-color : yellow;
}
</style>
