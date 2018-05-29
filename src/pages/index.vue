<template>
<div>
  <div class="sc-header">
    <div class="logo">
      <a href="#"></a>
    </div>
    <ul class="sc-top-nav">
      <li><a href="#" class="active">系统管理</a></li>
      <li><a href="#">内容管理</a></li>
      <li><a href="#">营销管理</a></li>
      <li><a href="#">订单管理</a></li>
      <li><a href="#">公众号管理</a></li>
    </ul>
    <div class="sc-login-area">
      <ul class="">
        <li><a href="">下载APP</a></li>
        <li><a href="">购物车</a></li>
        <li><a href="">消息</a></li>
        <li>
        <el-popover
          placement="top-start"
          width="200"
          trigger="click"
          :content="userCard">
          <a slot="reference"><img src="../assets/images/headimg.jpg"></a>
        </el-popover>
        <div ref="userCard">asdfasdf</div>
        </li>
      </ul>
    </div>
  </div>
  
  <div class="sc-nav"></div>

</div>
    
</template>

<script>

export default {
  name: 'index', 
  data () {
    return {
      userCard:"123"
    }
  },
  methods: {
  },
  mounted(){
    this.userCard=this.$refs.userCard.innerHTML
    console.log(this.$refs.userCard.innerHTML);
  }
}
</script>

<style scoped>
.sc-header{
  width: auto;
  height: 72px;
  padding:0 20px;
  position: relative;
  z-index: 800;
  background-color: #07111b;
}
.sc-header .logo{margin: 0 30px;float:left;}
.sc-header .logo a{
  display: block;
  height: 72px;
  width: 140px;
  background: url(../assets/images/logo.png) center center no-repeat;
  background-size:contain;
  overflow: hidden;
}
.sc-nav{
  height: 38px;
  line-height: 68px;
  background: #fff;
  box-shadow: 0 4px 4px 0 rgba(28,31,33,.1);
}
.sc-top-nav li{float:left;}
.sc-top-nav a{
    position: relative;
    padding: 0 25px;
    display: block;
    color: rgba(255,255,255,.6);
    text-align: center;
    font-size: 16px;
    height: 72px;
    line-height: 72px;
    font-weight: 400;
}
.sc-top-nav a:hover{color:#FFF;}
.sc-top-nav a.active{color:#FFF;}
.sc-login-area{position: relative;float:right;}
.sc-login-area  li{
  position: relative;

  height: 72px;
  line-height: 72px;
  color: rgba(255,255,255,.6);
  float:left;
}
.sc-login-area a{
  position: relative;
  padding: 0 15px;
  display: block;
  color: rgba(255,255,255,.6);
  text-align: center;
  font-size: 16px;
  height: 72px;
  line-height: 72px;
  font-weight: 400;
}
.sc-login-area a>img{
    width: 36px;
    height: 36px;
    border-color: #4d5559;
    border-radius: 50%;
    vertical-align: middle;
    display: inline-block;
}
</style>
