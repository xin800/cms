<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
*{
  margin:0;
  padding:0;
}
ul,li{list-style:none;}
html,body{
  width:100%;
  height:100%;
  font: 14px/1.5 "PingFang SC","微软雅黑","Microsoft YaHei",Helvetica,"Helvetica Neue",Tahoma,Arial,sans-serif;
}
#app{
  width:100%;
  height:100%;
  display:block;
}
a:link{text-decoration: none;}
a:hover{color:#FFF;}
</style>
