<template>
    <div id="app">  
      <keep-alive>
          <router-view v-if="$route.meta.keepAlive"></router-view>
      </keep-alive>
     <router-view v-if="!$route.meta.keepAlive"></router-view>
    </div>
</template>

<script>
  export default {
    name: 'App'
  }
</script>

<style>
  #app{
    height: 100%;
  }
 body{
       margin: 0;
       padding: 0;
       font-family:"Helvetica Neue",Helvetica,"PingFang SC","Hiragino Sans GB","Microsoft YaHei","微软雅黑",Arial,sans-serif;
  }
</style>
