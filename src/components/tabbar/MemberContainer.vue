<template>
  <div class="content">
    <div class="txh">
      <img class="tx" src="../../images/tx.jpg" alt="">
      <h3 class="yhm">Olivia</h3>
    </div>
   
    <div class="mine">
      <hr>
      <div class="mineComments memberch">
        <h4>我的</h4>
        <a href="#">收藏</a>
        <a href="#">评论</a>
        <a href="#">分享</a>
      </div>
      <hr>
      <div class="myOrder memberch">
        <h4>我的订单</h4>
        <a href="#">待付款</a>
        <a href="#">待发货</a>
        <a href="#">待收货</a>
        <a href="#">评价</a>
        <a href="#">退款/售后</a>
      </div>
     <hr>
      <div class="memberCenter memberch">
        <h4>会员中心</h4>

      </div>
      <hr>
     
      <div class="recommendation memberch">
        <h4>-你可能还喜欢-</h4>
      </div>

    </div>
   <mt-button type="danger" class="tcdl" size="large">退出登录</mt-button> 
  </div>
</template>

<script>
import { Button } from 'mint-ui';
</script>

<style lang="scss" scoped>

h3{
  color:black;
  padding-top: 0px;
}
.txh{
  border-radius: 50%;
 
}
.tx{
  height: 50px;
  width: 50px;
  margin-top: 20px;
  margin-left: 20px;
  border-radius: 50%;
  
 
}
.mine{
  color:black;
}
.tcdl{
 margin-bottom: 0px;
}
.memberch{
height: 100px;
}
</style>
