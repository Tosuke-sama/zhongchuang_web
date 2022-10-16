<template>
    <div class="main">
        <Font :TextBackground="'CONSULTATION CASE'" :TextFront="'咨询案例'"></Font>
        <div class="Carouseltext">
            我们了解一个优秀的职业规划对于大学生来说是多么迫切
        </div>
        <div class="Carousel">
            <el-carousel class="container" :interval="4000" type="card"  >
                <el-carousel-item class="box1" v-for="item in items" :key="item">
                    <div class="box">
                    <img :src="item.url" alt="" style="height:80%;width:100%; border-radius: 5px;">
                    <h3 class="boxtext" text="2xl" justify="center" >{{item.text}}</h3>
                    </div>
                </el-carousel-item>
            </el-carousel>
        </div>
    </div>
</template>
<script lang="ts">
    import Font from'@/components/Font.vue'
    export default({
        name:"Carousel",
        components:{
        Font,
      },
      data(){
        var items=[
        {
            "url":require("../../assets/workplace1.png"),
            "text":"了解市场运行规律很重要"
        },
        {
            "url":require("@/assets/workplace2.png"),
            "text":"对于长时间经济疲惫的市场来说，促销是很有用的刺激"
        },
        {
            "url":require("@/assets/workplace3.png"),
            "text":"运行着现有市场的不仅是经济，还有《国富论》。"
        }
    ]
    return{
        items
          }
      }
    })
</script>
<style scoped>
@media(min-width: 768px){
    .main{
    height: 800px;
    background-color: rgb(236, 236, 236);
}
.Carouseltext{
    margin-top:1%;
    margin-bottom: 2%;
    font-size: 23px;
}
.container{
    height: 100%;
}

.boxtext{
    font-size: 23px;
}
.Carousel{
    height: 65%;
    width: 70%;
    margin: auto;
}
.box1{
    height: 150%;
}
.box{
    height: 100%;
    /* background-color: rgb(184, 184, 184); */
}
}
@media(max-width: 768px){
.main{
    height: 500px;
    width:100%;
    background-color: rgb(236, 236, 236);
}
.container{
    height: 80%;
}

.Carouseltext{
    margin-top:1%;
    margin-bottom: 2%;
    font-size: 14px;
}
.Carousel{
    width: 99%;
    margin: auto;
}
.box1{
    height: 80%;
}
.boxtext{
    margin: 0;
    font-size: 15px;
    /* color: #ffffff;
    background-color: #000000; */
}

.box{
    height: 100%;
    /* background-color: rgb(184, 184, 184); */
}
}
/* .el-carousel__item h3 {
  color: #475669;
  opacity: 0.75;
  line-height: 200px;
  margin: 0;
  text-align: center;
} */

/* .el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
} */

</style>