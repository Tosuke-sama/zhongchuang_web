<template>
    <div class="box">
        <div class="left"
        >
            <div>
                <img src="@/assets/workplace2.png" alt="" class="imgleft">
            </div>
            <div class="title">
                {{titleleft}}
            </div>
            <div class="textbox">
                {{textleft}}
            </div>
        </div>
        <div class="middle"
            >
            <img src="@/assets/workplace1.png" alt="" class="imgmid">
            <div class="title">
                {{titlemid}}
            </div>
            <div class="textbox">
                {{textmid}}
            </div>
        </div>
        <div class="right"
        >
            <div>
                <img src="@/assets/workplace3.png" alt="" class="imgmid">
            </div>
            <div class="title">
                {{titleright}}
            </div>
            <div class="textbox">
                {{textright}}
            </div>
        </div>
    </div>
</template>
  
  <script lang="ts">
  export default({
      name:"contentnew",
      data() {
    return {
        titleleft:"为了企业未来的长久发展，做一些改变是理所应当的。",
        textleft:"2019年2月24日本周，我们开始推出新的视觉识别，以更好地表达我们是谁以及我们今天所做的事情。例如，我们公司五年前就没有一半以上的客户工作..",
        titlemid:"我们开始推出新的视觉识别，以更好地表达我们是谁以及我们今天所做的事情",
        textmid:"2019年2月24日本周，我们开始推出新的高级合伙人彼得达尔斯特罗姆说:‘我们认为对比描绘了我们的思想清晰度以及我们切入和提供真正重要的东西的能力。我们开始推出新的视觉识别，以更好地表达我们是谁以及我们今天所做的事情",
        titleright:"我们开始推出新的视觉识别，以更好地表达我们是谁以及我们今天所做的事情",
        textright:`2019年2月24日本周，我们开始推出新的视
觉识别，以更好地表达我们是谁以及我们今
天所做的事情。例如，我们公司五年前就没
有一半以上的客户工作..刷新包括更新的图形元素，新字体,新的调
色板以及数据可视化和摄影的改进方法。蓝

`
    }
  },


})
  </script>
  
  <style scoped>
    @media(min-width: 768px){
        .box{
            width: 70%;
            display: flex;
            flex-direction:row ;
            margin: auto;
        }
        .left{
            width: 50%;
            height: 55vh;
            text-align: left;
        }
        .left:hover{
            box-shadow: 0 0 8px 3px #999  ;
        }
        .imgleft{
            height: 42vh; 
            width:100%;
        }
        .middle{
            width: 25%;
            height: 55vh;
            margin-right:1rem ;
            margin-left:1rem ;
            text-align: left;
        }
        .middle:hover{
            box-shadow: 0 0 8px 3px #999  ;
        }
        .imgmid{
            height: 21vh; 
            width:100%;
        }
        .right{
            width: 25%;
            height: 55vh;
            text-align: left;
        }
        .right:hover{
            box-shadow: 0 0 8px 3px #999  ;
        }
        .title{
            font-size: 1.2rem;
            font-weight:bold;
            text-indent:2em;
            margin-right:1rem ;
            margin-left:1rem ;
        }
        .textbox{
            font-size: 1.1rem;
            text-indent:2em;
            margin-right:1rem ;
            margin-left:1rem ;
            color: rgb(135, 135, 135);
        }
        .box active{
            box-shadow: 0 0 5px 1px #999  ;
        }
    }
    @media(max-width: 768px){
        .box{
            width: 90%;
            display: flex;
            flex-direction:column ;
            margin: auto;
        }
        .left{
            width: 100%;
            height: 57vh;
            text-align: left;
        }
        .imgleft{
            height: 42vh; 
            width:100%;
        }
        .middle{
            margin-top: 1rem;
            margin-bottom: 1rem;
            width: 100%;
            height: 40vh;
            text-align: left;
        }
        .imgmid{
            height: 21vh; 
            width:100%;
        }
        .right{
            width: 100%;
            height: 40vh;
            text-align: left;
        }
        .title{
            font-size: 1rem;
            font-weight:bold;
            text-indent:2em;
            margin-right:1rem ;
            margin-left:1rem ;
        }
        .textbox{
            font-size: 0.3rem;
            text-indent:3em;
            margin-right:1rem ;
            margin-left:1rem ;
            color: rgb(135, 135, 135);
        }
    
    }
  </style>
  
  