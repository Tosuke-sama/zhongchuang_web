<template>
    <div class="golf">
    <div class="photo" ><img src="@/assets/img1.png" id="left"></div>
        <div class="intro" id="right">
        <h3>我们更新了我们的视觉效果</h3>
        <p>为了不使得企业或者公司的数据泄露，采用深度双重加密系统显得极其重要。</p>
    </div>
    <div style="clear:both"></div>
</div>
</template>
<script lang="ts">
const left:any =  document.querySelector('#left')as HTMLDivElement;
const right:any  = document.querySelector('#right') as HTMLDivElement;
// right.style.height=left.style.height
export default({
    name:"PhotoText",
})
</script>
<style>
    .photo{
        float:left;
        width:30%;
        padding-left:15%;
    }
    .intro{
        height: 100%;
        float:left;
        width:50%;
        background-color: aliceblue;
    }
    #left{
        width: 100%;
        height: 100%;
    }
</style>