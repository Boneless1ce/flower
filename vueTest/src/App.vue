<template>
  <div id="app">
    <router-view></router-view>
    <img src="./assets/logo.png">
   
    <index msg="222"></index>
    <div msg="aaa">111</div>

    <div class="m-tabbar">
      <div class="m-tabbar-item">
        <a href="">
          <span>首页</span>
        </a>
      </div>
      <div class="m-tabbar-item">
        <a href="">
          <span>搜索</span>
        </a>
      </div>
      <div class="m-tabbar-item">
        <a href="">
          <span>购物车</span>
        </a>
      </div>
      <div class="m-tabbar-item">
        <a href="">
          <span>关于</span>
        </a>
      </div>
      <div class="m-tabbar-item">
        <a href="">
          <span>我的</span>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import index from './components/index'
export default {
  name: 'App',
  components:{
    index
  }
}
</script>

<style>
*{
  margin:0;
  padding: 0;
  list-style: none;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.m-tabbar{
  display: flex;
  flex-direction: row;
  height: 50px;
  border-top: 1px solid #e5e5e5;
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
}
.m-tabbar-item{
  flex:1;
  height: 100%;
  line-height: 50px;
  
}
.m-tabbar-item a{
  text-decoration: none;
  color: #c8c8c8;
}
</style>
