<template>
      <div class="common-layout">
    <el-container>
      <el-header style="height: auto;"><Header :imgURL="require('@/assets/imgheader.png')"/>   </el-header>
      <el-main>
        <Font :TextBackground="'BUSINSESS REVIEW'" :TextFront="'商业评论'"></Font>
      <contentnew/>
       <div class="buttondiv">
          <el-button size="large" class="buttonClass" color="#000000" :dark="isDark">More<el-icon class="icon"><Right style="height:100%;width:100%" color="#FFFFFF" size="10" /></el-icon></el-button>
       </div>
       <Font :TextBackground="'EXPEPT COLUMN'" :TextFront="'专家专栏'"></Font>
       <PhotoText></PhotoText>
       <div class="buttondiv">
          <el-button size="large" class="buttonClass" color="#000000" :dark="isDark">More<el-icon><Right class="icon" color="#FFFFFF" size="10" /></el-icon></el-button>
       </div>
       <BgPhotoText></BgPhotoText>
       <Font :TextBackground="'TRAINING COURSE'" :TextFront="'培训课程'"></Font>
       <TrainText></TrainText>
       <el-button plain size="large" class="buttonClass" style="width:150px; margin: 3% 0;">More</el-button>
       <Carousel></Carousel>
      </el-main>
      <el-footer class="footer">
        <div class="footernum">
          <div style="
          font-size:23px;
          text-align: left;margin-top: 3.5%;margin-left: 25%;
          ">404-8820-5560 &nbsp;&nbsp;&nbsp;四川省成都市高新区二层108号</div>
          <div style="color: #aaaaaa;; font-size:20px;text-align: left;margin-left: 25%;margin-top: 1%;">Copyright © 2004-2007 |a.com 版权所有|咨询有风险，投资需谨慎 </div>
        </div>
        <div class="qrcode">
          <img src="@/assets/QRcode.png" alt="" style="height:60%;width: 11%;">
        </div>
      </el-footer>
    </el-container>
  </div>
</template>
<script lang="ts">
import Header from'@/components/Header.vue'
import contentnew from'@/components/index/ContentNew.vue'
import Font from'@/components/Font.vue'
import { defineComponent, reactive } from 'vue';
import PhotoText from '../components/PhotoText.vue';
import BgPhotoText from '@/components/index/BgPhotoText.vue';
import TrainText from '@/components/index/TrainText.vue';
import Carousel from'@/components/index/Carousel.vue'
export default{
    name:'index',
    setup(){
      const data = reactive({
        url: "imgheader.png",
      })
    },
    components:{
    Header,
    Font,
    PhotoText,
    BgPhotoText,
    TrainText,
    Carousel,
    contentnew
}
}
</script>
<style scoped>
@media(min-width: 768px){
  .body{
  margin:0px;
  width: 100%;
  padding: 0px;
}
.el-header {
  --el-header-padding: 0 0px;
}
.el-main{
  padding:0px;
}
.buttonClass {
  padding-top: 20px;
  padding-bottom: 20px;
  width: 250px;
  height: 60px;
  padding: 0;
  font-size: 25px;
}
.buttondiv{
  padding-top: 30px;
  padding-bottom: 30px;
}
.icon{
  width:20px;
  height:20px;
}
.footer{
  height: 150px;
  padding: 0;
  background-color: rgba(0, 0, 0, 0.786);
  display: flex;
  flex-direction: row;
  color: #ffffff;
}
.footernum{
  width: 60%;
  display: flex;
  flex-direction: column;
}
.qrcode{
  color: #aaaaaa;
  width: 40%;
  margin: auto;
}
}
@media(max-width: 768px){
  .body{
  margin:0px;
  width: 100%;
  padding: 0px;
}
.el-header {
  --el-header-padding: 0 0px;
}
.el-main{
  padding:0px;
}
.buttonClass {
  padding-top: 20px;
  padding-bottom: 20px;
  width: 30%;
  height: 50px;
  padding: 0;
  font-size: 20px;
}
.buttondiv{
  margin-top: 30px;
  margin-bottom: 30px;
}
.icon{
  width:20px;
  height:20px;
}
.footer{
  height: 150px;
  padding: 0;
  background-color: rgba(0, 0, 0, 0.786);
  display: flex;
  flex-direction: row;
  color: #ffffff;
}
.footernum{
  width: 60%;
  display: flex;
  flex-direction: column;
}
.qrcode{
  color: #aaaaaa;
  width: 40%;
  margin: auto;
}
}
</style>