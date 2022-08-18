<template>
      <div class="common-layout">
    <el-container>
      <el-header style="height: auto;"><Header :imgURL="require('@/assets/imgheader.png')"/>   </el-header>
      <el-main>
        <div style="font-size:70px;
        position:absolute;
        opacity:0.1;
        left:0;right:0;margin:0 auto;
        font-weight:bold;
        padding-top:20px
        ">
        BUSINSESS REVIEW</div>
        <div style="font-size: 60px; 
        font-weight:bold;
        padding-top: 50px;
        padding-bottom: 20px;
        ">
        商业评论</div>
       <Content/>
       <div>
          <el-button size="large" class="buttonClass" color="#000000" :dark="isDark">More<el-icon><Right class="icon" color="#FFFFFF" size="10" /></el-icon></el-button>
       </div>
      </el-main>
      <el-footer>Footer</el-footer>
    </el-container>
  </div>
</template>
<script lang="ts">
import Header from'@/components/Header.vue'
import content from'@/components/index/content.vue'
import { defineComponent, reactive } from 'vue';
import Content from '@/components/index/content.vue';
export default{
    name:'index',
    setup(){
      const data = reactive({
        url: "imgheader.png"
      })
    },
    components:{
    Header,
    content,
    Content
}
}
</script>
<style>
.el-header {
  --el-header-padding: 0 0px;
}
.buttonClass {
  padding-top: 20px;
  width: 250px;
  height: 60px;
  padding: 0;
  font-size: 25px;
}
.icon{
  width:10px;
  height:10px;
}
</style>