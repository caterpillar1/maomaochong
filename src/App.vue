<template>
  <div id="app">
    <div class="container">
      <div class="left">左边</div>
      <div class="main">中间</div>
      <div class="right">右边</div>
    </div>
    <div class="box"></div>
  </div>
</template>
<style>
  /* 1. flex布局 */
  .container{
    display:flex;
    justify-content: center;
    height: 200px;
    background: #eee;
  }
  .left {
    width: 200px;
    background-color: red;
    height: 100%;
  }
  .main {
    background-color: yellow;
    flex: 1; /*重点*/
  }
  .right {
    width: 200px;
    background-color: green;
  }
  .box{
    width:0px;
    height:0px;
    border: 50px solid;
    /*获得红色向右的箭头*/
    border-color:blue green orange red;
  }
</style>
