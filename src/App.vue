<template>
  <div class="header">
    <div class="logotext">
    <div class="logo">
      <img src="@/assets/logo.png" alt="logo图片">
    </div>
    <div class="text">
      中 和 同 创
    </div>
  </div>
    <div class="num">
     400-8820-8820
    </div>
    <div class="search">
      <input type="text" placeholder="输入关键词">
      <button></button>
    </div>
  </div>
  
<div id="nav1">
  <el-icon style="height:100%;width:8%;margin-right: 2%;"><More style="height:100%;width:100%" /></el-icon>
</div>
 <div id="nav">
    <el-menu
    router
    class="el-menu-demo"
    mode="horizontal"
    :ellipsis="false"
    background-color=#1689a0
    text-color="#FFFFFF"
  >
    <el-menu-item index="/"></el-menu-item>
    <div class="flex-grow"></div>
    <el-menu-item index="/index" style="margin-left:17%">首页</el-menu-item>
    <el-menu-item index="#">研究与洞察</el-menu-item>
    <el-menu-item index="/about">国企改革</el-menu-item>
    <el-menu-item index="/login">职能咨询</el-menu-item>
    <el-menu-item index="/login">管理与人才评测</el-menu-item>
    <el-menu-item index="/login">人才培养</el-menu-item>
    <el-menu-item index="/login">合作伙伴</el-menu-item>
    <el-menu-item index="/login" class="menu">联系我们</el-menu-item>
    <el-menu-item index="/login" class="menu">文化激励平台</el-menu-item>
  </el-menu>
  </div>
  
  <!-- <nav>
    <router-link to="/index">首页</router-link> |
    <router-link to="/about">About</router-link>
  </nav> -->
  <router-view />
</template>
<script lang="ts">
  export default {
    name: 'App',
    components: {

    },
    setup () {
      return {
      
      }
    },
    methods: {

  }
  }
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

@media(min-width: 768px){
  #nav1{
    display:none;
  }
nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
.header{
  height: 85px;
  margin-top:0px;
  line-height:85px;
  display: flex;
}
.logotext{
  height: 100%;
  width: 50%;
  display: flex;
}
.logo{
    /* float: left; */
    margin-left: 20%;
    vertical-align:middle;
}
.logo img{
  height: 60px;
  width: 60px;
  vertical-align:middle;
}
.text{
  margin-left: 1rem;
  /* float: left; */
  font-size: 30px;
  font-weight:bold;
}
.num{
  /* float: left; */
  margin-left:26%;
  font-size: 20px;
  font-weight:bold;
}
.search{
        /* float: left; */
        height: 85px;
        margin-left:5%; 
        text-align: center;
        display: flex;
       }
.search input{
        /* float: left; */
        width: 200px;
        height: 30px;
        border: 1px solid;
        color: #3f3f3f;
        font-size: 14px;
        /* padding-left: 15px; */
        margin: auto 0;
        /* margin-top: 23px; */
    }
.search button{
        /* float: left; */
        width: 35px;
        height: 35px;
        /* margin-top: 23px; */
        margin: auto 0;
        border: 1px;
        background-color: black;
        background-image: url('@/assets/search.png');
        background-size:100% 100%;
    }
.el-menu-demo li{
    padding-left: 1.5%;
    font-size: 18px;
    }
  }
    @media(max-width: 768px){
      #nav{
          display: none;
        }
      #nav1{
          height: 5vh;
          background-color: #ffffff;
          text-align: right;
          border: 0.5px solid;
        }
      .header {
          height: 85px;
          margin-top: 0px;
          line-height: 85px;
          display: flex;
        }
        .logotext{
          height: 100%;
          width: 50%;
          margin: auto;
          display: flex;
        }
        .logo {
          margin-left: 3%;
          vertical-align: middle;
        }
        .logo img {
          height: 50px;
          width: 50px;
          vertical-align: middle;
        }
        .text{
        margin-left: 2px;
        font-size: 25px;
        font-weight:bold;
        }
        .num{
        display: none;
        }
        .search{
          display: none;
        }
        .drawer {
        width: 100%;
        height: 100%;
        background: #fff;
}
       
    }
</style>
