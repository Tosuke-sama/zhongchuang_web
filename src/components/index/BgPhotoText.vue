<template>
    <div class='PhotoBg ' :style="{backgroundImage:'url('+require('../../assets/note.jpg')+')'}" style=" background-attachment: fixed;">
         <!-- <Font :TextBackground="'IMFORMATION'" :TextFront="'研究报告'" id="fontBg" style="color:#FFFFFF;"></Font> -->
        <div class="bg1">{{TextBackground}}</div>
        <div class="ft1">{{TextFront}}</div>
        <div style="color:#FFFFFF">《新泽没有夏天》是李京介“时间、世界与冒险”系列的第一卷，讲述了少年叶瑾介与步行在未来的少女、时间鸟、以及</div>
        <div class="content1" style="z-index:10;" >
            <div class='wrap'>
            <a href="">为了挽回世界线的变动，叶瑾介决定让自己分裂......<el-icon><Right class="icon" color="#000000" size="3" /></el-icon></a>
            <a href="">为了挽回世界线的变动，叶瑾介决定让自己分裂......<el-icon><Right class="icon" color="#000000" size="3" /></el-icon></a>
            <a href="">为了挽回世界线的变动，叶瑾介决定让自己分裂......<el-icon><Right class="icon" color="#000000" size="3" /></el-icon></a>
            <a href="">为了挽回世界线的变动，叶瑾介决定让自己分裂......<el-icon><Right class="icon" color="#000000" size="3" /></el-icon></a>
            <a href="">为了挽回世界线的变动，叶瑾介决定让自己分裂......<el-icon><Right class="icon" color="#000000" size="3" /></el-icon></a>
            <a href="">为了挽回世界线的变动，叶瑾介决定让自己分裂......<el-icon><Right class="icon" color="#000000" size="3" /></el-icon></a>
        </div>
        <div style="padding-top: 20px;">
            <el-button size="large" class="buttonClass"  color="#000000" :dark="isDark">More<el-icon><Right class="icon" color="#FFFFFF" size="10" /></el-icon></el-button>
        </div>
        </div>
    </div>
</template>
<script lang="ts">
import Font from "@/components/Font.vue"
export default({
    name:'BgPhotoText',
    data() {
    return {
        TextBackground: 'IMFORMATION',
        TextFront:"研究报告"
    }
  },
    setup(){
        const url='../assets/img1.png';
        var TextBackground="6666"
        return{url}
    },
    components:{
        Font,
    }
})
</script>
<style scoped>
.PhotoBg{
    z-index:-10;
    height: 800px;
    width:100%;
}
.content1{
    height: 60%;
    width: 70%;
    margin: 2% auto;
    background-color: #ffffff;
}
.wrap{
    height: 65%;
    width: 100%;
    padding-top: 15px;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
}
.wrap a{
    width: 50%;
    display:block;
    margin:auto;
    color: #000000;
}
.bg1{
    font-size:70px;
    position:absolute;
    opacity:0.8;
    left:0;right:0;margin:0 auto;
    font-weight:bold;
    padding-top:20px;
    color: #000000;
    z-index: 1;
}
.ft1{
    font-size: 60px; 
    font-weight:bold;
    position: relative;
    padding-top: 50px;
    padding-bottom: 20px;
    color: #ffffff;
    z-index: 10;
}

</style>