<template>
      <div class="common-layout">
    <el-container>
      <el-header style="height: auto;"><Header :imgURL="require('@/assets/imgheader.png')"/>   </el-header>
      <el-main>
        <Font :TextBackground="'BUSINSESS REVIEW'" :TextFront="'商业评论'"></Font>
       <Content/>
       <div class="buttondiv">
          <el-button size="large" class="buttonClass" color="#000000" :dark="isDark">More<el-icon><Right class="icon" color="#FFFFFF" size="10" /></el-icon></el-button>
       </div>
       <Font :TextBackground="'EXPEPT COLUMN'" :TextFront="'专家专栏'"></Font>
       <PhotoText></PhotoText>
      </el-main>
      <el-footer>Footer</el-footer>
    </el-container>
  </div>
</template>
<script lang="ts">
import Header from'@/components/Header.vue'
import content from'@/components/index/content.vue'
import Font from'@/components/Font.vue'
import { defineComponent, reactive } from 'vue';
import Content from '@/components/index/content.vue';
import PhotoText from '../components/PhotoText.vue';
export default{
    name:'index',
    setup(){
      const data = reactive({
        url: "imgheader.png",
      })
    },
    components:{
    Header,
    content,
    Content,
    Font,
    PhotoText
}
}
</script>
<style>
.el-header {
  --el-header-padding: 0 0px;
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
   padding-top: 20px;
  padding-bottom: 20px;
}
.icon{
  width:10px;
  height:10px;
}
</style>