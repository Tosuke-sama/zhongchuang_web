<template>
    <div class="golf">
    <div class="photo" ><img src="@/assets/img1.png" id="left"></div>
        <div class="intro" id="right">
        <h3 class="titlept">我们更新了我们的视觉效果</h3>
        <p class="textpt">为了不使得企业或者公司的数据泄露，采用深度双重加密系统显得极其重要。</p>
    </div>
    <div style="clear:both"></div>
</div>
</template>
<script lang="ts">
export default({
    name:"PhotoText",
})
</script>
<style scoped>
  @media(min-width: 768px){
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
    .titlept{
        font-size:2rem;
        padding-bottom: 10%;
        font-weight: bold;
    }
    .textpt{
        font-size:1.5rem
    }
  }
  @media(max-width: 768px){
    .golf{
    display: flex;
    flex-direction:column;
    justify-content:center;
    padding-top: 2%;
    }
    .photo{
        width:90%;
        height: 30vh;
        margin: auto;
    }
    .intro{
        width:90%;
        background-color:  #f0f0f5;
        margin: auto;
        height: 17vh;
    }
    .intro > *{
        margin: 0;
    }
    #left{
        width: 100%;
        height: 100%;
    }
    .titlept{
        font-size:1.5rem;
        padding-top: 7%;
        padding-bottom: 5%;
        font-weight: bold;
        margin-right:1rem ;
        margin-left:1rem ;
    }
    .textpt{
        font-size:1rem;
        padding-bottom: 1vh;
        margin-right:1rem ;
        margin-left:1rem ;
    }
  }

</style>