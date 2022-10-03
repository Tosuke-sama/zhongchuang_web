<template>
    <div class="golf">
    <div class="photo" ><img src="@/assets/img1.png" id="left"></div>
        <div class="intro" id="right">
        <h3 style="font-size:25px;padding-bottom: 10%;">我们更新了我们的视觉效果</h3>
        <p>为了不使得企业或者公司的数据泄露，采用深度双重加密系统显得极其重要。</p>
    </div>
    <div style="clear:both"></div>
</div>
</template>
<script lang="ts">
export default({
    name:"PhotoText",
})
</script>
<style>
    .golf{
    display: flex;
    flex-direction:row;
    justify-content:center;
    padding-top: 2%;
    }
    .photo{
        width:30%;
    }
    .intro{
        width:30%;
        background-color:  #f0f0f5;
        padding-top: 5%;
        padding-left:20px;
        padding-right:20px;
    }
    .intro > *{
        margin: 0;
    }
    #left{
        width: 100%;
        height: 100%;
    }
</style>