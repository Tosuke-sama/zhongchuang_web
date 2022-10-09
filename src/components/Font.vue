<template>
    <div class="bg">{{TextBackground}}</div>
    <div class="ft">{{TextFront}}</div>
</template>
<script lang="ts">
export default({
    name:"Font",
    props:["TextBackground","TextFront","BgColor","FtColor"],
})
</script>
<style>
@media(min-width: 768px){
    .bg{
    font-size:70px;
    position:absolute;
    opacity:0.1;
    left:0;right:0;margin:0 auto;
    font-weight:bold;
    padding-top:20px
}
.ft{
    font-size: 60px; 
    font-weight:bold;
    padding-top: 50px;
    padding-bottom: 20px;
    position: relative;
}
}

@media(max-width: 768px){
    .bg{
    font-size:40px;
    position:absolute;
    opacity:0.1;
    left:0;right:0;margin:0 auto;
    font-weight:bold;
    padding-top:20px
}
.ft{
    font-size: 40px; 
    font-weight:bold;
    padding-top: 40px;
    padding-bottom: 30px;
    position: relative;
}
}
</style>