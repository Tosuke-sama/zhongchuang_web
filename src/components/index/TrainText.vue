<template>
    <div>
        <div class="main">
            <div class="imgtext" 
            @mouseover="mouseOver($event)"
            @mouseleave="mouseLeave($event)"
            :style="active"
            >
                <img src="@/assets/workplace1.png" alt="" class="trainimg">
                <div class="traintitle" >
                    构建技术型生态系统
                </div>
                <div class="traintext">来自五大洲的三十多位同志加入了他们的行列</div>
            </div>
            <div class="imgtext" style="margin:0 3%;"
            @mouseover="mouseOver($event)"
            @mouseleave="mouseLeave($event)"
            :style="active"
            >
                <img src="@/assets/workplace2.png" alt="" class="trainimg">
                <div class="traintitle">
                    构建技术型生态系统
                </div>
                <div class="traintext">来自五大洲的三十多位同志加入了他们的行列</div>
            </div>
            <div class="imgtext"  
            @mouseover="mouseOver($event)"
            @mouseleave="mouseLeave($event)"
            :style="active"
            >
                <img src="@/assets/workplace3.png" alt="" class="trainimg">
                <div class="traintitle">
                    构建技术型生态系统
                </div>
                <div class="traintext">来自五大洲的三十多位同志加入了他们的行列</div>
            </div>
        </div>
    </div>
</template>
<script  lang="ts">
export default({
    name:"TrainText",
    data() {
    return {
        active: "",
    }
  },
    methods: {
        mouseOver($event){
            $event.currentTarget.className = "imgtext active";
            $event.currentTarget.firstElementChild.className="trainimg ativeimg"
        //   this.active = "";
        //   var acps = this.$refs.acp
        //   acps.style.color="red"
        },
        mouseLeave($event){
            $event.currentTarget.className = "imgtext";
            $event.currentTarget.firstElementChild.className="trainimg"
        }
},
})
</script>
<style scoped>
@media(min-width: 768px){
    .main{
    height: 400px;
    width: 70%;
    /* background-color:red; */
    display: flex;
    flex-direction: row;
    /* padding: 0 15%; */
    margin: auto;
}
.imgtext{
    height: 100%;
    width:33%;
}
.trainimg{
    height: 70%;
    width: 100%;
}
.traintitle{
    /* width: 70%; */
    text-align: left;
    font-family: Arial,"Microsoft Yahei", "微软雅黑";
    font-size: 25px;
    font-weight:bold;
    margin: 5% 0 5% 5%;
}
.traintext{
    text-align: left;
    margin-left: 5%;
    /* width: 70%; */
}
.active{
    /* opacity:0.9; */
    background-color: rgba(255, 72, 72, 0.996);
    box-shadow: 0 0 5px 1px #999  ;
    color: #ffffff;
}
.ativeimg{
    filter: opacity(80%);
}
}
@media(max-width: 768px){
    
    .main{
    height: 35vh;
    width: 90%;
    /* background-color:red; */
    display: flex;
    flex-direction: row;
    /* padding: 0 15%; */
    margin: auto;
}
.imgtext{
    height: 90%;
    width:33%;
}
.trainimg{
    height: 50%;
    width: 100%;
}
.traintitle{
    /* width: 70%; */
    text-align: left;
    font-family: Arial,"Microsoft Yahei", "微软雅黑";
    font-size: 18px;
    font-weight:bold;
    margin: 5% 0 5% 5%;
}
.traintext{
    font-size: 15px;
    text-align: left;
    margin-left: 5%;
    /* width: 70%; */
}
.active{
    /* opacity:0.9; */
    background-color: rgba(255, 72, 72, 0.996);
    box-shadow: 0 0 5px 1px #999  ;
    color: #ffffff;
}
.ativeimg{
    filter: opacity(80%);
}
}
</style>